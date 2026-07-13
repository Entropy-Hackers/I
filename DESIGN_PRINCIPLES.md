# Design Principles of I

**Version 1 · 2026**

This document records the architectural decisions that shape I and the reasoning behind them: why I is designed the way it is, what alternatives were considered, and what led to the choices made.

The Design Principles serve two purposes. They let future contributors understand the reasoning behind existing architecture rather than reverse-engineering intent from implementation. And they provide a basis for evaluating proposed changes: a change that conflicts with a stated principle requires either a principled argument for overriding the principle or a revision of the principle itself.

These principles can be changed through the normal governance process. The invariants — the properties that no future version of the Constitution may surrender — are stated in `CONSTITUTION.md`, Article 43.

---

## 1. Protocols before platforms

**Principle:** I is defined by its protocols rather than by any software platform, service, or organisation.

**Reasoning:** Platforms fail. Services are discontinued. Organisations change. A protocol, correctly written, can persist across many generations of implementation. Defining I through protocols rather than platforms means any sufficiently motivated party can implement I independently, without depending on any existing implementation or organisation.

This is how the internet works. HTTP, TCP/IP, and DNS can be implemented by anyone, which is why no single company can end the internet by ceasing to operate. I is designed with the same property.

**Implication:** When a protocol and a platform conflict, the protocol is authoritative. No platform-level decision constitutes a change to the protocol.

---

## 2. No centre

**Principle:** I has no central server, central repository, or central authority.

**Reasoning:** A centre is a vulnerability — it can be destroyed, controlled, corrupted, or defunded. Each of these failure modes has occurred in scientific infrastructure. A network without a centre survives the ending of any single node.

The propagation obligation — every Host must propagate to at least two peers — implements this principle. It keeps the observational record distributed across the network rather than held in any one place.

**What this means in practice:** There is no master database of observations, and no single server that must be running for I to function. The Constitutional Archive at `github.com/Entropy-Hackers/I` is the canonical source for definitions and protocols, but it is itself a git repository that any party can mirror. If GitHub disappeared, the repository would continue wherever it had been mirrored.

---

## 3. Instruments as documents

**Principle:** An Instrument is a document. Hardware is a Realisation of the Instrument.

**Reasoning:** Hardware fails, becomes obsolete, is discontinued — an Instrument defined by its hardware dies with the hardware. An Instrument defined by a document, a precise published specification, can be reimplemented on any hardware meeting the specification's requirements.

This separation also enables comparability across time. Two devices built ten years apart, by different manufacturers, in different countries, realising the same Instrument version, produce observations that can be directly compared. The shared specification guarantees the comparability, independent of hardware identity.

**What this means in practice:** Instrument specifications must be written with sufficient precision that a competent engineer who has never seen the original device can build a conforming Realisation. A specification that requires access to the original authors for clarification needs more precision.

---

## 4. Signed observations

**Principle:** Every Observation is cryptographically signed by the Host that produced it. Verification requires trusting only the signature, never an intermediary.

**Reasoning:** A database record can be modified by whoever controls the database. A cryptographically signed observation can only be modified by whoever holds the signing key, and any modification is detectable, because the signature stops verifying.

Over the decades during which the observational record accumulates, the question of whether a particular observation was actually produced by the stated Host at the stated time will matter. Cryptographic signatures answer that question durably; institutional assurances ("trust us, we wouldn't alter the records") answer it only as long as the institution does.

**What this means in practice:** The signing infrastructure must be implemented before Hosts begin producing Observations. Unsigned observations cannot be retrospectively signed with the same guarantees, so the decision to require signing from the start has to be made at the start.

---

## 5. Raw data is immutable and primary

**Principle:** Raw Data is never modified after observation. Processed, corrected, and quality-controlled products are derived from it, alongside it, never in place of it.

**Reasoning:** The theoretical frameworks within which observations are interpreted change over time. What seems like noise today may be signal tomorrow; what seems like a systematic error today may be a real phenomenon. Discarding raw data in favour of processed products forecloses the possibility of reinterpretation.

The history of science includes many cases where raw data, re-examined under new theoretical frameworks, yielded insights unavailable to the original observers — possible only because the raw data survived.

**What this means in practice:** Preserving raw data for the long term costs more than preserving processed products alone. I accepts this cost as necessary: the value of the raw record over a century is worth the storage cost.

---

## 6. The century horizon

**Principle:** Every architectural decision is evaluated against the question: does this still work in a hundred years?

**Reasoning:** The phenomena I is designed to observe — atmospheric composition, ecological change, long-duration environmental processes — operate on timescales of decades to centuries. The observational record only becomes fully valuable once it spans these timescales. Architectural decisions that work well for ten years but fail in thirty are wrong decisions for I.

This principle allows current technology to be used freely, provided there is a documented path for migrating to successor technologies without losing the observational record.

**What this means in practice:** Data formats must be documented completely enough to be decoded without access to the original software. Protocols must be versioned in a way that preserves backward compatibility with existing observations. The constitutional history is preserved even as the Constitution is amended.

---

## 7. Minimum necessary governance

**Principle:** I governs itself as little as possible. Governance is achieved through architecture wherever possible.

**Reasoning:** Governance structures are expensive to maintain, slow to act, and susceptible to capture by the interests of those most active in them. A decision encoded in a protocol is more resilient than a decision made by a committee, because it depends on neither the committee's continued existence nor its good judgment.

The goal is governance by architecture: systems designed so that correct behaviour is the path of least resistance, and incorrect behaviour is detectable and attributable.

**What this means in practice:** When a new rule seems necessary, the first question is whether it can be encoded in a protocol instead. If it can, it should be. A governance process is appropriate only when the situation genuinely requires human judgment, and remains the last resort.

---

## 8. Equality of Hosts, asymmetry of record

**Principle:** All Hosts have equal authority. The quality of a Host's record — its history of observations, calibration, and propagation — is public and speaks for itself.

**Reasoning:** In centralised scientific infrastructure, authority correlates with size, funding, and institutional prestige, reproducing existing inequalities: well-funded institutions in wealthy regions gain more influence over what is observed, how, and by whom. I is designed to break this correlation.

The mechanism is simple: authority in I derives only from protocol conformance and observation quality, both public and verifiable. A Host operating for one month with impeccable calibration carries more observable credibility than a Host operating for ten years with gaps and calibration failures. The record is the credential.

**What this means in practice:** The governance process cannot give any Host special voting rights, veto powers, or preferential treatment based on its size, age, or funding. A governance structure that does so has been captured.

---

## 9. Openness as architecture

**Principle:** Openness in I is embedded in the architecture, beyond the reach of any single governance decision to reverse.

**Reasoning:** Policies change when the people who made them leave, when political winds shift, when commercial pressures mount. An architectural commitment to openness is harder to reverse: reversing it would require changing the protocols themselves, which must follow the declared change process, which is a public record.

I achieves architectural openness through: CC0 licensing of all constitutional documents and instrument specifications; protocol specifications that require no licence to implement; observation formats readable without proprietary software; a constitutional archive that any party can mirror.

**What this means in practice:** Any proposed protocol or instrument specification requiring a licence to implement, or making observations inaccessible without proprietary software, is incompatible with I regardless of any governance decision to adopt it.

---

## 10. Succession over continuity

**Principle:** I is designed for succession — for what happens when people leave and others take their place with the same obligations and standing.

**Reasoning:** Continuity of participants can't be guaranteed; people and organisations leave. Succession can be engineered, because it is a protocol obligation rather than a hope.

The Host lineage system — the record of which Hosts established which others — is the mechanism for succession. When a Host ceases to operate, the Host it established continues. When a founding participant leaves, the participants they trained continue. The knowledge and practice propagate even as the specific people change.

**What this means in practice:** Hosts are expected to establish at least one successor before ceasing operation. This is currently a strong expectation rather than a hard protocol requirement, and should become one in a future protocol version.

---

*Design Principles of I · Version 1 · 2026 · CC0 · github.com/Entropy-Hackers/I*
