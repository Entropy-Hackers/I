# Design Principles of I

**Version 1 · 2026**

This document records the architectural decisions that shape I and the reasoning behind them. It is not a protocol specification. It is a record of intent: why I is designed the way it is, what alternatives were considered, and what led to the choices made.

The Design Principles serve two purposes. They allow future contributors to understand the reasoning behind existing architecture rather than having to reverse-engineer intent from implementation. They provide a basis for evaluating proposed changes: a change that conflicts with a stated principle requires either a principled argument for overriding the principle or a revision of the principle itself.

These principles are not invariants. They can be changed through the normal governance process. The invariants — the properties that no future version of the Constitution may surrender — are stated in `CONSTITUTION.md`, Article 43.

---

## 1. Protocols before platforms

**Principle:** I is defined by its protocols, not by any software platform, service, or organisation.

**Reasoning:** Platforms fail. Services are discontinued. Organisations change. A protocol, if correctly written, can persist across many generations of implementation. The value of defining I through protocols rather than platforms is that any sufficiently motivated party can implement I independently, without depending on any existing implementation or organisation.

This is how the internet works. HTTP, TCP/IP, and DNS are not controlled by any single company. Anyone can implement them. As a result, no single company can end the internet by ceasing to operate. I is designed with the same property.

**Implication:** When a protocol and a platform conflict, the protocol is authoritative. No platform-level decision constitutes a change to the protocol.

---

## 2. No centre

**Principle:** I has no central server, central repository, or central authority.

**Reasoning:** A centre is a vulnerability. It can be destroyed, controlled, corrupted, or defunded. Each of these failure modes has occurred in scientific infrastructure. A network without a centre cannot be ended by ending any single node.

The propagation obligation — every Host must propagate to at least two peers — is the mechanism that implements this principle. It ensures that the observational record is distributed across the network, not held in any one place.

**What this means in practice:** There is no master database of observations. There is no single server that must be running for I to function. The Constitutional Archive at `github.com/Entropy-Hackers/I` is the canonical source for definitions and protocols, but it is itself a git repository that can be mirrored by any party. If GitHub ceased to exist, the repository would continue wherever it had been mirrored.

---

## 3. Instruments as documents

**Principle:** An Instrument is a document, not a device. Hardware is a Realisation of the Instrument.

**Reasoning:** Hardware fails, becomes obsolete, is discontinued. If an Instrument is defined by its hardware, it dies when the hardware does. If an Instrument is defined by a document — a precise, published specification — it can be reimplemented on any hardware that can meet the specification's requirements.

This separation also enables comparability across time. Two devices built ten years apart, by different manufacturers, in different countries, realising the same Instrument version, produce observations that can be directly compared. The comparability is guaranteed by the shared specification, not by hardware identity.

**What this means in practice:** Instrument specifications must be written with sufficient precision that a competent engineer who has never seen the original device can build a conforming Realisation. If a specification requires access to the original authors for clarification, it is not sufficiently precise.

---

## 4. Signed observations, not trusted databases

**Principle:** Every Observation is cryptographically signed by the Host that produced it. Verification does not require trusting any intermediary.

**Reasoning:** A database record can be modified by whoever controls the database. A cryptographically signed observation can only be modified by whoever holds the signing key — and any modification is detectable, because the signature will no longer verify.

Over the decades during which the observational record accumulates, the question of whether a particular observation was actually produced by the stated Host at the stated time will matter. Institutional trust — "trust us, we wouldn't alter the records" — is not a durable answer. Cryptographic signatures are.

**What this means in practice:** The signing infrastructure must be implemented before Hosts begin producing Observations. Unsigned observations cannot be retrospectively signed in a way that provides the same guarantees. The decision to require signing from the start is a decision that cannot be deferred.

---

## 5. Raw data is immutable and primary

**Principle:** Raw Data is never modified after observation. Processed, corrected, and quality-controlled products are derived from Raw Data. They do not replace it.

**Reasoning:** The theoretical frameworks within which observations are interpreted change over time. What seems like noise today may be signal tomorrow. What seems like a systematic error today may be a real phenomenon. If raw data is discarded in favour of processed products, the possibility of reinterpretation is foreclosed.

The history of science includes many cases where raw data, re-examined under new theoretical frameworks, yielded insights unavailable to the original observers. This can only happen if the raw data was preserved.

**What this means in practice:** Storage is not free. Preserving raw data for the long term costs more than preserving processed products. I accepts this cost as necessary. The value of the raw record over a century is worth the storage cost.

---

## 6. The century horizon

**Principle:** Every architectural decision is evaluated against the question: does this still work in a hundred years?

**Reasoning:** The phenomena that I is designed to observe — atmospheric composition, ecological change, long-duration environmental processes — operate on timescales of decades to centuries. The observational record only becomes fully valuable when it spans these timescales. Architectural decisions that produce a system that works well for ten years but fails in thirty are wrong decisions for I.

This principle does not mean that I cannot use current technology. It means that when current technology is used, there must be a documented path for migrating to successor technologies without losing the observational record.

**What this means in practice:** Data formats must be documented completely enough that they can be decoded without access to the original software. Protocols must be versioned in a way that preserves backward compatibility with existing observations. The constitutional history must be preserved even as the Constitution is amended.

---

## 7. Minimum necessary governance

**Principle:** I governs itself as little as possible. Governance is achieved through architecture wherever possible.

**Reasoning:** Governance structures are expensive to maintain, slow to act, and susceptible to capture by the interests of those most active in them. A decision encoded in a protocol is more resilient than a decision made by a committee, because it does not depend on the committee's continued existence or good judgment.

The goal is governance by architecture: systems designed so that correct behaviour is the path of least resistance, and incorrect behaviour is detectable and attributable.

**What this means in practice:** When a new rule seems necessary, the first question to ask is whether the rule can be encoded in a protocol instead. If it can, it should be. If it cannot — if the situation genuinely requires human judgment — then a governance process is appropriate. But governance should be the last resort, not the first.

---

## 8. Equality of Hosts, asymmetry of record

**Principle:** All Hosts have equal authority. No Host has more authority than any other. The quality of a Host's record — its history of observations, calibration, and propagation — is public and speaks for itself.

**Reasoning:** In centralised scientific infrastructure, authority correlates with size, funding, and institutional prestige. This produces networks that reflect existing inequalities: well-funded institutions in wealthy regions have more influence over what is observed, how, and by whom. I is designed to break this correlation.

The mechanism is simple: authority in I derives only from protocol conformance and observation quality, both of which are public and verifiable. A Host that has been operating for one month with impeccable calibration has more observable credibility than a Host that has been operating for ten years with gaps and calibration failures. The record is the credential.

**What this means in practice:** The governance process cannot give any Host special voting rights, veto powers, or preferential treatment based on its size, age, or funding. If this becomes necessary for practical reasons, it is a sign that the governance structure has been captured.

---

## 9. Openness as architecture, not policy

**Principle:** Openness in I is not a policy that could be reversed by a governance decision. It is embedded in the architecture.

**Reasoning:** Policies change when the people who made them leave, when political winds shift, when commercial pressures mount. An architectural commitment to openness is harder to reverse: it would require changing the protocols themselves, which must follow the declared change process, which is a public record.

I achieves architectural openness through: CC0 licensing of all constitutional documents and instrument specifications; protocol specifications that cannot require a licence to implement; observation formats that do not require proprietary software to read; a constitutional archive that can be mirrored by any party.

**What this means in practice:** Any proposed protocol or instrument specification that would require a licence to implement, or that would make observations inaccessible without proprietary software, is incompatible with I regardless of any governance decision to adopt it.

---

## 10. Succession over continuity

**Principle:** I is designed for succession, not for continuity of any particular set of participants.

**Reasoning:** Continuity implies that the same people and organisations keep operating. Succession implies that when people leave, others take their place, with the same obligations and the same standing. I cannot be designed around continuity, because continuity cannot be guaranteed. It can be designed around succession, because succession is a protocol obligation.

The Host lineage system — the record of which Hosts established which others — is the mechanism for succession. When a Host ceases to operate, the Host it established continues. When a founding participant leaves, the participants they trained continue. The knowledge and practice propagate, even as the specific people change.

**What this means in practice:** Hosts are expected to establish at least one successor before ceasing operation. This is not currently a hard protocol requirement, but it is a strong expectation and should become a requirement in a future protocol version.

---

*Design Principles of I · Version 1 · 2026 · CC0 · github.com/Entropy-Hackers/I*
