# Constitution of I

**Version 1 · 2026**  
Released under CC0. No rights reserved.

---

## Preamble

The world produces signals continuously.

Temperature, pressure, chemistry, light, sound, motion, composition — at every point on the earth's surface, at every moment, the world is doing something measurable. Most of these signals dissolve into the past unrecorded, because no one has built infrastructure adequate to the task.

The infrastructure that exists was built for a different world: a time when instruments required large buildings and permanent staff, when data required central archives, when science required institutional gatekeeping. That world has changed faster than the infrastructure has kept up.

I is an attempt to build infrastructure adequate to the world as it is: a world in which a device the size of a hand can make a measurement comparable to one made in a laboratory, in which a network of ten thousand independent parties can collectively observe phenomena that no single institution could afford to monitor, in which the protocols that coordinate human activity can be defined openly and implemented by anyone.

I is an attempt to change the infrastructure of that world.

This Constitution defines what I is, what it must remain regardless of how the world around it changes, and the principles that govern how it may change — including which parts may never change.

This Constitution has no owner: no organisation owns it, no government ratifies it, no authority enforces it. It is enforced by the practice of those who implement it, and by the simple fact that something failing to conform to what I means cannot be called I.

---

## Part One · What I Is

### Article 1 · I has no legal form

I has no company, association, foundation, institute, consortium, headquarters, staff, bank account, or legal personality.

I is a distributed scientific infrastructure: a set of open protocols, a community of Hosts, a body of Instruments, and an accumulating record of Observations of the world.

The absence of legal personhood is a design decision. Legal entities are subject to the laws of the jurisdictions in which they are registered, to the politics of their time, to the interests of those who control them. I must outlast any particular jurisdiction, political moment, or interest group.

What I is can be stated, implemented, and maintained without any entity that can be sued, taxed, dissolved, or acquired.

### Article 2 · I outlives its founders

The founding participants of I — the individuals and organisations who wrote these documents, defined these protocols, and operated the first Instruments — hold no permanent authority to speak for I.

I is defined by its Constitution, its protocols, and its Observations. No founding participant has authority beyond any other participant. No lineage of participation creates hierarchy. History creates memory; power is a separate matter entirely.

If every founding participant ceased to participate, I would continue in the hands of those who remained. If all participants ceased, I would exist in its archive: in the Observations already made, the protocols already published, the Instruments already defined.

This document will still describe what I is after everyone who wrote it is gone.

### Article 3 · I is a living infrastructure

I remains unfinished — at the writing of this Constitution, at its supersession, and always.

I grows as Hosts join the network. I deepens as Instruments are defined. I accumulates as Observations are made and propagated. I matures as Analysis transforms Observations into Knowledge.

The word *living* here is practical rather than biological: I is a practice that requires continuous participation to remain real, that changes because the world changes and understanding grows, that has a past, a present, and an open future.

---

### Article 4 · What I is for

I exists to enable humanity to collectively observe reality — the whole of it, across its full spatial extent and temporal duration, regardless of what is currently considered scientifically important or currently funded.

The scope of this purpose exceeds what I can achieve at any moment. That is appropriate. An infrastructure whose purpose is fully achieved has stopped being necessary. The purpose is a direction, not a destination.

### Article 5 · The timescale of I

I is designed to operate across centuries. This is a design requirement that shapes every decision made in this Constitution and in the protocols that implement it.

Decisions that are convenient for a decade but fragile across a century are wrong decisions for I, even when they are right decisions for everything else.

The test of any architectural choice is whether it still works — or at minimum leaves a recoverable record — once the organisations, technologies, and funding structures of the present moment no longer exist.

---

## Part Two · The Vocabulary of I

The following definitions form the conceptual architecture of I. To use these words in the senses defined here is to think within the framework of I; to use them in other senses is to think about something else.

All capitalised uses of these terms throughout I documents refer to these definitions.

### Article 6 · Observation

An Observation is a record of a measurement made by a conforming Instrument at a specific location and time, in accordance with the Instrument's protocol.

An Observation is **singular**: it records what happened at one place and one time, distinct from an average, a summary, or a model output.

An Observation is **immutable**: once recorded and propagated, it stays fixed. Errors can be noted and flagged, but the record itself endures.

An Observation is **signed**: it carries the cryptographic signature of the Host that produced it, verifiable by any party without trusting any intermediary.

An Observation is **attributed**: it identifies the Instrument and the version of that Instrument's protocol that produced it.

The immutability of Observations is the most important single property of I. Knowledge changes. Analysis changes. Interpretation changes. Theory changes. The signal that the world produced at a particular moment stays fixed. Every future generation must be able to return to the Observation and reinterpret it under frameworks that do not yet exist.

An altered Observation becomes a fabrication.

### Article 7 · Raw Data

Raw Data is the unmodified output of a sensor or measurement process, as received from the physical world, prior to any transformation.

Raw Data is the substrate of Observation. An Observation wraps Raw Data in provenance: it adds the identity of the Host, the identity of the Instrument, the timestamp, the location, the signature. The Raw Data within an Observation is the unaltered signal.

Raw Data enters an Observation exactly as measured. Quality control, averaging, calibration correction, and interpolation belong to Analysis, which produces derived products alongside the original.

### Article 8 · Instrument

An Instrument is a protocol that specifies how a class of Observations is to be produced.

An Instrument specifies: the physical quantity or phenomenon to be measured; the method of measurement, precisely enough for independent implementation; the conditions under which the measurement is valid; the format of the output Raw Data; the calibration procedure; the known sources of systematic error.

An Instrument is a document; hardware is a realisation of it. Many different physical devices, built at different times, in different places, by different parties, may realise the same Instrument. If they conform to the Instrument's protocol, their Observations are comparable. The document can be copied, read, implemented, versioned, and cited without any physical object.

**Instrument 000000** is the Instrument that defines what an Instrument is. It produces no Observations of the physical world; it is the constitutional document of the Instrument system. Every Instrument in I derives its formal status from Instrument 000000.

### Article 9 · Host

A Host is any entity that operates one or more Instrument realisations, records the resulting Observations, propagates those Observations according to the propagation protocol, and accepts the responsibilities defined in the Host Protocol.

A Host may be an individual, a family, a school, a laboratory, a university, a company, a city, a research institute, or any other entity capable of sustained responsible operation.

All Hosts are equal in authority within I. Size, wealth, institutional prestige, political influence, and duration of participation create no hierarchy among Hosts. A Host established yesterday has identical standing to the first Host.

What differs between Hosts is their record: the history of Observations they have produced, the accuracy and consistency of their calibration, the reliability of their propagation. This record is public. It creates reputation, distinct from authority.

### Article 10 · Identity

Every participant in I — every Host, every Instrument author, every contributor — holds a cryptographic identity: a public/private key pair.

The public key is the identity: globally unique, self-generated, requiring no issuing authority and no registry.

All Observations are signed by the identity of the Host that produced them. All Instrument specifications are signed by the identity of their authors. All protocol changes are signed by the identities of their proposers.

Identity persists permanently, and the record of what an identity has done is auditable by anyone. Identity authenticates actions rather than persons — the connection between a key pair and a human being is a social fact that sits outside what I manages.

### Article 11 · Analysis

Analysis is any process that takes Observations as input and produces a derived product as output.

An Analysis is reproducible when: the input Observations are identified precisely, by their unique IDs; the procedure is specified completely, as executable code; the computational environment is described sufficiently that the procedure can be re-executed by any party with access to the input Observations.

Analysis that cannot be reproduced from its stated inputs is assertion, distinct from Analysis in the sense of I.

Analysis may change as understanding grows. New Analysis of old Observations is one of the principal mechanisms by which I produces new Knowledge from existing records, possible only because the Observations remain available and unaltered.

### Article 12 · Knowledge

Knowledge is a structured claim about the world that is supported by one or more Analyses, which are in turn supported by one or more Observations, which are in turn produced by one or more Instruments.

The value of Knowledge in I is inseparable from the transparency of this chain. A Knowledge claim with no traceable chain to Observations is opinion.

Knowledge claims can be disputed, revised, extended, and superseded. When they are, the revision and its basis are recorded alongside the original claim — neither is deleted. The history of a Knowledge claim is part of the claim.

### Article 13 · Protocol

A Protocol is a complete, public specification of a procedure that any conforming party can implement independently, producing results comparable to those of any other conforming party.

In I, protocols govern: how Instruments are specified and versioned; how Observations are recorded, signed, and formatted; how Hosts propagate Observations to peers; how identities are established and maintained; how protocol changes are proposed, deliberated, and adopted.

A protocol is defined by its text, which is public. Any implementation conforming to the text is a valid implementation, freely available to anyone without licence or fee.

### Article 14 · Propagation

Propagation is the mechanism by which Observations spread across the network of Hosts without passing through any centre.

When a Host records an Observation, it propagates it to its declared peers. Those peers propagate it to their peers. The Observation reaches every Host that has declared an interest in it without any central node deciding who receives what.

Propagation is a protocol obligation: a Host that fails to propagate Observations to its declared peers is failing to fulfil the Host Protocol.

The propagation structure ensures that no single failure destroys the observational record. An Observation that has propagated to multiple Hosts survives the failure of any one of them.

### Article 15 · Stewardship

Stewardship is the disposition of a Host toward its Observations.

A Host holds the Observations it produces as steward, for the duration of its availability commitment, rather than as owner. Ownership implies the right to destroy, to withhold, to sell; stewardship implies the obligation to preserve, to propagate, to hand over.

A Host whose availability commitment expires propagates its Observations more widely, ensures that other Hosts hold them, and records its own cessation in the host log.

Stewardship is the ethical disposition that holds the network together when no other obligation does.

### Article 16 · Memory

Memory is the accumulated body of Observations in I.

Memory grows continuously as new Observations are added, and holds steady otherwise: Observations are immutable and permanent. Memory is distributed, held across all Hosts, propagated so that no single location or institution holds it exclusively.

Memory is the purpose of I materialised. Every Observation added to Memory is a record of the world at a specific moment, preserved for every future generation that might want to ask questions of it.

An unrecorded signal is lost forever. A recorded signal that is later destroyed is lost forever. A recorded signal that has propagated survives any single loss.

### Article 17 · Time

I takes time seriously as a design variable.

Most infrastructure is designed for the needs of the present. I is designed equally for the needs of those who will inhabit the future.

The observational record has value that compounds over time. An Observation made today has one value now and a different, larger value in fifty years, when it can be compared with fifty years of subsequent Observations.

Decisions that optimise for the present at the cost of the future are wrong decisions for I.

The minimum temporal horizon for any architectural decision in I is one century.

---

### Article 18 · Continuity

Continuity is the property of I that ensures its function persists across changes of technology, organisation, funding, and personnel.

Continuity is achieved through: propagation, which ensures no single failure destroys the record; protocol publication, which ensures any party can implement I independently; constitutional versioning, which preserves the history of I's self-definition alongside the Observations it generates; the Host lineage system, which lets the network survive the departure of any participant through established successors.

The architecture produces continuity. No organisation guarantees it.

---

## Part Three · The Principles of I

### Article 19 · Openness is constitutional

I is open. Openness is the condition under which I is I — as fundamental to its identity as any property in this Constitution.

Openness means: all protocols are public and freely implementable; all Instrument specifications are public and freely implementable; all Observations are accessible to any party that can reach a Host; all Analysis is reproducible by any party with access to the inputs; all governance deliberations are public records.

Every Observation in I remains available regardless of commercial interest, national security, institutional priority, or personal preference. Withholding one removes it from I, leaving only a private record.

### Article 20 · Distributed by necessity

I has no centre, because a centre is a vulnerability.

A network with a centre can be destroyed by destroying the centre. It can be controlled by controlling the centre. It can be corrupted by corrupting the centre. It can be defunded by defunding the centre.

Each of these failure modes has occurred in scientific infrastructure. I is designed so that none of them can destroy the whole.

The distributed architecture is the correct response to the historical record of centralised scientific infrastructure and its failure modes.

### Article 21 · Observations are their own end

Observations are collected because the world is producing signals that would otherwise dissolve into the past unrecorded.

The Observation is the end point of the observational act. Analysis, Knowledge, and policy may follow from it, and I supports all of these — but they remain secondary to the Observation itself.

An infrastructure that treats Observations as means to other ends will discard Observations that fail to serve current ends — the central failure mode of existing scientific data infrastructure. I treats Observations as ends, preserved for their own sake, in case they are needed for purposes that are not yet imaginable.

### Article 22 · Protocols before implementations

The protocols of I outrank any implementation of them. An implementation can be replaced; a protocol, correctly written, can persist across many generations of implementation.

When a protocol and an implementation conflict, the protocol is authoritative.

When a protocol must be revised, the revision is made to the protocol first, and implementations follow. No implementation-level change constitutes a change to the protocol.

This principle has a practical consequence: protocols are written with the care of constitutional documents rather than software documentation. They are precise, conservative, and stable, changing slowly and with full deliberation.

### Article 23 · Trust through verification

I asks everyone to verify, rather than asking anyone to trust any party.

The cryptographic signature on an Observation requires only the ability to verify it against the Host's public key.

The reproducibility requirement on Analysis requires only the ability to re-run the Analysis on the same inputs and verify the output.

The public nature of the constitutional archive requires only the ability to read the history and verify that changes followed declared process.

The architecture earns trust in I. This is the only form of trust that survives the replacement of every current participant by someone who has never heard of them.

### Article 24 · Minimum governance

I governs itself as little as possible and as much as necessary.

Governance is expensive. It is slow. It is susceptible to capture by the interests of those who participate most actively in it. More governance rarely produces better outcomes; often it produces worse ones.

The minimum necessary governance for I is: a process for revising protocols; a process for accepting new Instrument definitions; a process for resolving disputes about Host conduct; a record of all governance decisions, publicly available.

Everything else is governed by the protocols themselves. A decision encoded in a protocol can be captured by an interest group only by changing the protocol itself, which must follow declared process, which is a public record.

The goal is governance by architecture rather than by committee.

### Article 25 · Authority is never inherited

Participation in I, however long, creates no special authority.

The first Host has no more authority than the thousandth. The author of this Constitution has no more authority than any future participant who has read it. The organisation that established the first Instrument has no more authority than any future Instrument author.

Authority in I derives only from: conformance to the protocols, which any party can verify, and the quality of the Observations produced, which is public record.

History creates memory and reputation — valuable, but a separate thing from authority.

### Article 26 · Responsibility is always personal

While authority in I is never inherited, responsibility is.

A Host that establishes another Host accepts a responsibility of mentorship: to ensure the new Host understands what I requires and has the capacity to meet those requirements.

A Host that ceases operation discharges its responsibilities by ensuring its Observations have propagated to sufficient other Hosts, by recording its cessation in the host log, and by notifying the Hosts to which it propagated.

Responsibility attaches to the entity that accepted it, not to any institution or successor. If the entity dissolves, the responsibility goes undischarged, and the host log records what was done and what was left undone.

---

## Part Four · Instruments

### Article 27 · What makes something an Instrument of I

An Instrument of I is a published, versioned, open protocol specification that has been accepted through the Instrument registration process defined in the governance documents.

To be accepted, an Instrument specification must:

- define a specific, measurable physical quantity or phenomenon
- specify the measurement methodology precisely enough for independent implementation without access to the authors
- define the output format completely and formally
- describe known sources of systematic error and their magnitudes
- specify a calibration procedure performable without specialised equipment beyond what is generally available
- include at least one reference implementation and at least one independent validation dataset

A document meeting these requirements and accepted through the registration process is an Instrument. A device implementing this document is a realisation of the Instrument — the two remain distinct.

### Article 28 · Instrument 000000

Instrument 000000 is the meta-instrument: the Instrument that defines what an Instrument is.

It produces no Observations of the physical world. Its function is to define the formal properties that all Instruments must have, in a form that is itself an Instrument: structured, versioned, and subject to the same governance as every other Instrument.

Every Instrument in I is formally derived from Instrument 000000. Changes to Instrument 000000 propagate implications to all Instruments. The history of Instrument 000000 is part of the history of every Instrument.

### Article 29 · Instrument versioning

An Instrument version is a complete, self-contained specification: a new document that explicitly states its relationship to all previous versions of the same Instrument, rather than a patch on a previous version.

A new version must explicitly state: which previous versions it is compatible with, and why; what has changed from the most recent previous version; what analysis demonstrates the comparability of Observations made under different compatible versions.

Compatibility is demonstrated, never assumed.

An Observation references the exact version of the Instrument that produced it. Two Observations made under different versions of an Instrument are comparable only to the extent that the version history documents.

### Article 30 · Instruments cannot be retired

An Instrument that has produced Observations is permanent.

It can be deprecated: marked as superseded, with a recommendation to use a newer version. It can be annotated: with corrections, clarifications, or warnings about known systematic errors discovered after publication. It stays in the archive.

The reason matches the reason Observations are immutable. Every Observation references the Instrument that produced it. Removing the Instrument would leave the Observation uninterpretable: a signal without a specification.

---

## Part Five · Hosts

### Article 31 · What it means to be a Host

To become a Host is to accept a set of responsibilities toward the observational record, toward the network of Hosts, and toward the future.

These responsibilities are operational requirements: to operate Instruments in conformance with their protocols; to record Observations in the canonical format; to sign Observations with the Host's identity key; to propagate Observations to declared peers; to maintain a public operational log; to preserve Raw Data for the duration of the stated availability commitment; to record cessation and propagate remaining Observations before ceasing to operate.

A Host meeting these requirements is a Host. A Host falling short is in breach of the Host Protocol, recorded in the network's public record. This Constitution prescribes no punishment — the record itself is the consequence.

### Article 32 · The equality of Hosts

All Hosts are equal. This is an architectural constraint.

No governance structure in I may give any Host authority over any other Host by virtue of size, wealth, duration of participation, institutional prestige, geographic location, or political influence.

What differs is the record, which is public and speaks for itself.

### Article 33 · Host lineages

A Host may establish another Host. The establishing Host takes responsibility for ensuring the new Host understands the requirements of I and has the capacity to meet them.

This creates a lineage: a public record of which Hosts established which others. Lineages preserve institutional memory, recording the propagation of practice and understanding across the history of I.

Lineages record history rather than power. The new Host owes nothing to the establishing Host beyond what the protocols require of every Host, and the establishing Host holds no authority over the new Host.

### Article 34 · The geographic obligation

The purpose of I — to enable humanity to collectively observe reality — depends on Hosts reaching beyond wealthy regions.

The phenomena most important to observe are often in the places least served by existing monitoring infrastructure. The geographic distribution of Hosts is a primary measure of whether I is doing what it says it is doing.

The network's coverage map is a moral map. Where it is blank, the world is unobserved.

---

## Part Six · Governance

### Article 35 · The purpose of governance in I

Governance in I exists to maintain the integrity of the protocols, to allow I to evolve without losing its identity, and to resolve disputes in a manner consistent with the principles of this Constitution.

Its mandate stops there. Directing the network, allocating resources, ranking participants, and representing I to external parties fall outside it.

### Article 36 · Governance by protocol

The primary mechanism of governance in I is the protocol.

A protocol defines what is valid. A Host either conforms to the protocol or falls into breach — conformance is verifiable by any party, and no governance body needs to make a judgment.

This is the most resilient form of governance in I: it depends only on the continued availability of the protocol text and the ability of Hosts to read and implement it, rather than on the continued existence of any committee, the good judgment of any individual, or the integrity of any institution.

### Article 37 · Protocol change process

Protocols change through a process that is: open — any participant may propose a change; public — all proposals and deliberations are recorded; deliberate — a minimum period for review is required; conservative — backward compatibility is strongly preferred; demonstrated — changes must have running implementations before adoption.

A protocol change with no implementation remains a hypothesis. A protocol change with a running implementation, demonstrated compatibility with the existing observational record, and rough consensus among active participants becomes a candidate for adoption.

Rough consensus means the absence of sustained, principled objection that has not been addressed, falling short of unanimous agreement.

### Article 38 · The constitutional amendment process

This Constitution may be amended, because the world changes and understanding grows. No part of it is permanently immune to amendment.

Constitutional amendment requires: a documented proposal with a full statement of reasons; a deliberation period of no less than one year; demonstrated support from Hosts across at least three distinct geographic regions; an explicit statement of what the amendment changes and why the change is consistent with the spirit of I.

An amendment that would make I depend on any single organisation, technology, or jurisdiction is an attempt to end I, and is invalid.

### Article 39 · What governance must never become

Governance in I must never become: a membership organisation with exclusive authority; a body that can prevent participation by conforming parties; a vehicle for the interests of large or wealthy participants at the expense of small or less wealthy ones; a mechanism for centralising the observational record; a source of revenue for its operators.

Any governance structure in I that acquires one of these properties becomes incompatible with this Constitution, and participants owe its decisions no recognition.

### Article 40 · Dispute resolution

Disputes between Hosts are resolved by appeal to the protocols.

If a Host believes another Host is in breach of a protocol, it states the breach precisely, with reference to the protocol text, and submits the statement to the public governance record. The accused Host may respond. The community of Hosts may deliberate. The outcome is a public record.

This Constitution prescribes no sanctions — the public record is the consequence. Hosts retain the right, under the Host Protocol, to individually stop propagating with a Host found in repeated breach; this is a choice available to them, not a punishment administered by any authority.

---

## Part Seven · The Constitutional History of I

### Article 41 · This Constitution has a history

This document is Version 1 of the Constitution of I, written in 2026. It will be amended, and every version will be preserved in the constitutional archive — the history of this Constitution is part of I.

The history of I begins with the first Observation ever recorded under an I protocol; that Observation is the true founding moment. Documents can be written before there is anything to document. An Observation can only be made in the present tense.

### Article 42 · Version 1 records its own limitations

This Constitution was written at a particular moment in history, by a small number of people, with the knowledge and limitations of that moment.

It will contain errors and omissions. It will contain principles that seem obvious now and mistaken in fifty years. It will fail to anticipate developments that will seem obvious in fifty years and are unimaginable now.

These are precisely the reasons to build in the capacity to amend it. The amendment process reflects the plain acknowledgement that a living infrastructure requires a living constitution.

### Article 43 · The invariants

Whatever changes in future versions of this Constitution, the following properties must be preserved.

> **I has no owner.**
> No individual, organisation, government, or any other entity may own I, own the observational record of I, or own the protocols that define I. The observational record is the common heritage of humanity, and no version of this Constitution may permit any party to privatise, enclose, or make it exclusive in whole or in part.

> **Observations are immutable.**
> No version of this Constitution may permit the alteration or deletion of Observations. Observations may be annotated, flagged, and contextualised by new knowledge, but they stay as recorded.

> **The protocols are open.**
> No version of this Constitution may permit the creation of a protocol that any conforming party cannot implement freely, without licence, fee, or permission.

> **All Hosts are equal.**
> No version of this Constitution may create permanent hierarchy among Hosts based on any property other than their record of conduct, which is public, auditable, and the same standard for all.

> **The constitutional history is permanent.**
> No version of this Constitution may permit the deletion of any previous version. The history of I's self-definition is part of I: it may be annotated, but it stays in the record permanently.

---

## Part Eight · Closing Articles

### Article 44 · The limits of this Constitution

This Constitution cannot enforce itself. There is no court, no government, no police standing behind it. Its authority rests entirely on the willingness of those who implement I to implement it consistently with what this document says.

This is simply how all constitutions work in practice — most are additionally backed by state power, and this one relies on practice alone.

The strength of this Constitution is that it describes something genuinely valuable to implement correctly: an infrastructure that produces trustworthy, permanent, open records of the world. Parties who implement it incorrectly may still produce something useful; they will have produced something other than I.

### Article 45 · The function of this Constitution

This Constitution establishes a shared vocabulary.

It defines what counts as an Observation, a conforming Host, a valid Instrument, and I itself. By fixing these definitions in a document that is itself part of I's permanent record, this Constitution lets anyone, at any time, determine whether any particular thing is consistent with what I is.

That is the function of a constitution: definition rather than enforcement, meaning rather than power.

### Article 46 · The invitation

I begins with the first Observation.

Before the first Observation, I is a set of documents and a set of intentions. After the first Observation, I is a record. The record grows. The record persists. The record becomes the most important thing about I.

This Constitution is addressed to the people who will make those Observations: the Hosts who will calibrate instruments, check sensors, maintain logs, propagate records, and do the quiet, unglamorous, essential work of attending to the world.

To them, and to every person who will read this document after all of us are gone, this Constitution says:

> The world was producing signals before you arrived.  
> It will produce signals after you are gone.  
> What you can do, in the interval, is attend to some of them,  
> record what you find, and pass the record on.  
>  
> That is what I is for.  
> That is what you are for, if you choose to participate.  
>  
> The rest is protocol.

---

*Constitution of I · Version 1 · 2026 · CC0 · github.com/Entropy-Hackers/I*
