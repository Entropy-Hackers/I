# Constitution of I

**Version 1 · 2026**  
Released under CC0. No rights reserved.

---

## Preamble

The world produces signals continuously.

Temperature, pressure, chemistry, light, sound, motion, composition — at every point on the earth's surface, at every moment, the world is doing something measurable. Most of these signals dissolve into the past unrecorded. Not because recording them is impossible, but because no one has built infrastructure adequate to the task.

The infrastructure that exists was built for a different world: for a time when instruments required large buildings and permanent staff, when data required central archives, when science required institutional gatekeeping. That world has changed. The infrastructure has not.

I is an attempt to build infrastructure adequate to the world as it is: a world in which a device the size of a hand can make a measurement comparable to one made in a laboratory, in which a network of ten thousand independent parties can collectively observe phenomena that no single institution could afford to monitor, in which the protocols that coordinate human activity can be defined openly and implemented by anyone.

I is not a project within that world. It is an attempt to change the infrastructure of that world.

This Constitution defines what I is. It defines what I is not. It defines what I must remain, regardless of how the world around it changes. It defines the principles that govern how I may change, and the principles that govern what may not change at all.

No organisation owns this Constitution. No government ratifies it. No authority enforces it. It is enforced by the practice of those who implement it, and by the impossibility of calling something I that does not conform to what I means.

---

## Part One · What I Is

### Article 1 · I is not an organisation

I is not a company, association, foundation, institute, consortium, or any other form of legal entity. I has no headquarters, no staff, no bank account, no legal personality.

I is a distributed scientific infrastructure: a set of open protocols, a community of Hosts, a body of Instruments, and an accumulating record of Observations of the world.

The absence of legal personhood is not a limitation. It is a design decision. Legal entities are subject to the laws of the jurisdictions in which they are registered, to the politics of their time, to the interests of those who control them. I must outlast any particular jurisdiction, political moment, or interest group.

What I is can be stated, implemented, and maintained without any entity that can be sued, taxed, dissolved, or acquired.

### Article 2 · I is not defined by its current participants

The founding participants of I — the individuals and organisations who wrote these documents, defined these protocols, and operated the first Instruments — do not own I and do not speak for I permanently.

I is defined by its Constitution, its protocols, and its Observations. No founding participant has authority that another participant does not have. No lineage of participation creates hierarchy. History creates memory. It does not create power.

If every founding participant ceased to participate, I would continue in the hands of those who remained. If all participants ceased, I would exist in its archive: in the Observations already made, the protocols already published, the Instruments already defined.

This document will still describe what I is after everyone who wrote it is gone.

### Article 3 · I is a living infrastructure

I is not finished. It was not finished when this Constitution was written. It will not be finished when this Constitution is superseded.

I grows as Hosts join the network. I deepens as Instruments are defined. I accumulates as Observations are made and propagated. I matures as Analysis transforms Observations into Knowledge.

The word *living* here does not mean biological. It means that I is not a monument but a practice: something that requires continuous participation to remain real, that changes because the world changes and because understanding grows, that has a past, a present, and an open future.

---

### Article 4 · What I is for

I exists to enable humanity to collectively observe reality.

Not a particular aspect of reality. Not the aspects currently considered scientifically important. Not the aspects currently funded. Reality, as it is, across its full spatial extent and temporal duration.

The scope of this purpose exceeds what I can achieve at any moment. That is appropriate. An infrastructure whose purpose is fully achieved is an infrastructure that has stopped being necessary. The purpose is a direction, not a destination.

### Article 5 · The timescale of I

I is designed to operate across centuries.

This is not an aspiration. It is a design requirement that shapes every decision made in this Constitution and in the protocols that implement it.

Decisions that are convenient for a decade but fragile across a century are wrong decisions for I, even when they are right decisions for everything else.

The test of any architectural choice is not whether it works now. It is whether it still works — or at minimum leaves a recoverable record — when the organisations, technologies, and funding structures of the present moment no longer exist.

---

## Part Two · The Vocabulary of I

The following definitions are not merely terminological. They are the conceptual architecture of I. To use these words in the senses defined here is to think within the framework of I. To use them in other senses is to think about something else.

All capitalised uses of these terms throughout I documents refer to these definitions.

### Article 6 · Observation

An Observation is a record of a measurement made by a conforming Instrument at a specific location and time, in accordance with the Instrument's protocol.

An Observation is **singular**: it records what happened at one place and one time. It is not an average, a summary, or a model output.

An Observation is **immutable**: once recorded and propagated, it cannot be altered. Errors in Observation can be noted and flagged. They cannot be erased.

An Observation is **signed**: it carries the cryptographic signature of the Host that produced it. Any party can verify the signature without trusting any intermediary.

An Observation is **attributed**: it identifies the Instrument and the version of that Instrument's protocol that produced it.

The immutability of Observations is the most important single property of I. Knowledge changes. Analysis changes. Interpretation changes. Theory changes. The signal that the world produced at a particular moment does not change. Every future generation must be able to return to the Observation and reinterpret it under frameworks that do not yet exist.

An Observation that has been altered is no longer an Observation. It is a fabrication.

### Article 7 · Raw Data

Raw Data is the unmodified output of a sensor or measurement process, as received from the physical world, prior to any transformation.

Raw Data is the substrate of Observation. An Observation wraps Raw Data in provenance: it adds the identity of the Host, the identity of the Instrument, the timestamp, the location, the signature. The Raw Data within an Observation is the unaltered signal.

No quality control, averaging, calibration correction, or interpolation is applied to Raw Data before it becomes part of an Observation. These operations belong to Analysis. They produce derived products. They do not modify the original.

### Article 8 · Instrument

An Instrument is a protocol that specifies how a class of Observations is to be produced.

An Instrument specifies: the physical quantity or phenomenon to be measured; the method of measurement, precisely enough for independent implementation; the conditions under which the measurement is valid; the format of the output Raw Data; the calibration procedure; the known sources of systematic error.

An Instrument is not hardware. Hardware is a realisation of an Instrument. Many different physical devices, built at different times, in different places, by different parties, may realise the same Instrument. If they conform to the Instrument's protocol, their Observations are comparable.

An Instrument is a document. The document is the Instrument. The document can be copied, read, implemented, versioned, and cited without any physical object.

**Instrument 000000** is the Instrument that defines what an Instrument is. It produces no Observations. It is the constitutional document of the Instrument system. Every Instrument in I derives its formal status from Instrument 000000.

### Article 9 · Host

A Host is any entity that operates one or more Instrument realisations, records the resulting Observations, propagates those Observations according to the propagation protocol, and accepts the responsibilities defined in the Host Protocol.

A Host may be an individual, a family, a school, a laboratory, a university, a company, a city, a research institute, or any other entity capable of sustained responsible operation.

All Hosts are equal in authority within I. Size, wealth, institutional prestige, political influence, and duration of participation create no hierarchy among Hosts. A Host established yesterday has identical standing to the first Host.

What differs between Hosts is their record: the history of Observations they have produced, the accuracy and consistency of their calibration, the reliability of their propagation. This record is public. It creates reputation, not authority.

### Article 10 · Identity

Every participant in I — every Host, every Instrument author, every contributor — holds a cryptographic identity: a public/private key pair.

The public key is the identity. It is globally unique. It is self-generated. No authority issues it. No registry must be consulted to create it.

All Observations are signed by the identity of the Host that produced them. All Instrument specifications are signed by the identity of their authors. All protocol changes are signed by the identities of their proposers.

Identity does not expire. The record of what an identity has done is permanent and auditable by anyone.

Identity does not authenticate persons in the social or legal sense. It authenticates actions. The connection between a key pair and a human being is a social fact that I does not manage.

### Article 11 · Analysis

Analysis is any process that takes Observations as input and produces a derived product as output.

An Analysis is reproducible when: the input Observations are identified precisely, by their unique IDs; the procedure is specified completely, as executable code; the computational environment is described sufficiently that the procedure can be re-executed by any party with access to the input Observations.

An Analysis that cannot be reproduced from its stated inputs is not Analysis in the sense of I. It is assertion.

Analysis may change as understanding grows. New Analysis of old Observations is one of the principal mechanisms by which I produces new Knowledge from existing records. This is only possible if the Observations remain available and unaltered.

### Article 12 · Knowledge

Knowledge is a structured claim about the world that is supported by one or more Analyses, which are in turn supported by one or more Observations, which are in turn produced by one or more Instruments.

The value of Knowledge in I is inseparable from the transparency of this chain. A Knowledge claim with no traceable chain to Observations is not Knowledge. It is opinion.

Knowledge claims can be disputed, revised, extended, and superseded. When they are, the revision and its basis are recorded alongside the original claim. Neither is deleted. The history of a Knowledge claim is part of the claim.

### Article 13 · Protocol

A Protocol is a complete, public specification of a procedure that any conforming party can implement independently, producing results comparable to those of any other conforming party.

In I, protocols govern: how Instruments are specified and versioned; how Observations are recorded, signed, and formatted; how Hosts propagate Observations to peers; how identities are established and maintained; how protocol changes are proposed, deliberated, and adopted.

A protocol is defined by its text. The text is public. Any implementation conforming to the text is a valid implementation. No licence, fee, or permission is required to implement a protocol of I.

### Article 14 · Propagation

Propagation is the mechanism by which Observations spread across the network of Hosts without passing through any centre.

When a Host records an Observation, it propagates it to its declared peers. Those peers propagate it to their peers. The Observation reaches every Host that has declared an interest in it without any central node deciding who receives what.

Propagation is not a courtesy. It is a protocol obligation. A Host that does not propagate Observations to its declared peers is not fulfilling the Host Protocol.

The propagation structure ensures that no single failure destroys the observational record. An Observation that has propagated to multiple Hosts cannot be destroyed by the failure of any one of them.

### Article 15 · Stewardship

Stewardship is the disposition of a Host toward its Observations.

A Host is not the owner of the Observations it produces. A Host is the steward of those Observations for the duration of its availability commitment.

The distinction is not semantic. Ownership implies the right to destroy, to withhold, to sell. Stewardship implies the obligation to preserve, to propagate, to hand over.

A Host whose availability commitment expires does not discard its Observations. It propagates them more widely, ensures that other Hosts hold them, and records its own cessation in the host log.

Stewardship is the ethical disposition that holds the network together when no other obligation does.

### Article 16 · Memory

Memory is the accumulated body of Observations in I.

Memory grows continuously as new Observations are added. Memory never diminishes: Observations are immutable and permanent.

Memory is distributed: it is held across all Hosts, propagated so that no single location or institution holds it exclusively.

Memory is the purpose of I materialised. Every Observation added to Memory is a record of the world at a specific moment, preserved for every future generation that might want to ask questions of it.

The loss of any Observation is permanent. What has not been recorded cannot be recovered. What has been recorded but destroyed cannot be recovered. What has been recorded and propagated can survive any single loss.

### Article 17 · Time

I takes time seriously as a design variable.

Most infrastructure is designed for the needs of the present. I is designed for the needs of the present and for the needs of those who will inhabit the future.

The observational record has value that compounds over time. An Observation made today has one value now and a different, larger value in fifty years, when it can be compared with fifty years of subsequent Observations.

Decisions that optimise for the present at the cost of the future are wrong decisions for I.

The minimum temporal horizon for any architectural decision in I is one century.

---

### Article 18 · Continuity

Continuity is the property of I that ensures its function persists across changes of technology, organisation, funding, and personnel.

Continuity is achieved through: propagation, which ensures no single failure destroys the record; protocol publication, which ensures any party can implement I independently; constitutional versioning, which ensures the history of I's self-definition is preserved alongside the Observations it generates; the Host lineage system, which ensures the network can survive the departure of any participant by having established successors.

Continuity is not guaranteed by any organisation. It is produced by the architecture.

---

## Part Three · The Principles of I

### Article 19 · Openness is not a feature. It is a condition.

I is open.

This is not a design choice among alternatives. It is the condition under which I is I. A version of I that is not open is not I.

Openness means: all protocols are public and freely implementable; all Instrument specifications are public and freely implementable; all Observations are accessible to any party that can reach a Host; all Analysis is reproducible by any party with access to the inputs; all governance deliberations are public records.

No Observation in I may be withheld on grounds of commercial interest, national security, institutional priority, or personal preference. An Observation that is withheld is not an Observation in I. It is a private record.

### Article 20 · Distributed by necessity, not preference

I has no centre because a centre would be a vulnerability.

A network with a centre can be destroyed by destroying the centre. It can be controlled by controlling the centre. It can be corrupted by corrupting the centre. It can be defunded by defunding the centre.

Each of these failure modes has occurred in scientific infrastructure. I is designed so that none of them can destroy the whole.

The distributed architecture is not a concession to technical fashion. It is the correct response to the historical record of centralised scientific infrastructure and its failure modes.

### Article 21 · Observations are ends, not means

Observations are not collected in order to produce papers, support grant applications, or satisfy reporting requirements.

Observations are collected because the world is producing signals that would otherwise dissolve into the past unrecorded.

The Observation is the end point of the observational act. What Analysis does with the Observation, what Knowledge emerges from it, what policy follows — these are valuable and I supports them. But they are secondary to the Observation itself.

An infrastructure that treats Observations as means to other ends will discard Observations that do not serve current ends. This is the central failure mode of existing scientific data infrastructure.

I treats Observations as ends. They are preserved for their own sake, in case they are needed for purposes that are not yet imaginable.

### Article 22 · Protocols before implementations

The protocols of I are more important than any implementation of them.

An implementation can be replaced. A protocol, if correctly written, can persist across many generations of implementation.

When a protocol and an implementation conflict, the protocol is authoritative.

When a protocol must be revised, the revision is made to the protocol first. Implementations follow. No implementation-level change constitutes a change to the protocol.

This principle has a practical consequence: protocols are written with the care of constitutional documents, not software documentation. They are precise, conservative, and stable. They change slowly and with full deliberation.

### Article 23 · Trust through verification, not authority

I does not ask anyone to trust any party. It asks everyone to verify.

The cryptographic signature on an Observation does not require trust in the Host that produced it. It requires only the ability to verify the signature against the Host's public key.

The reproducibility requirement on Analysis does not require trust in the analyst. It requires only the ability to re-run the Analysis on the same inputs and verify the output.

The public nature of the constitutional archive does not require trust in those who maintain it. It requires only the ability to read the history and verify that changes followed declared process.

Trust in I is earned by the architecture, not claimed by the participants. This is the only form of trust that survives the replacement of every current participant by someone who has never heard of them.

### Article 24 · Minimum governance

I governs itself as little as possible and as much as necessary.

Governance is expensive. It is slow. It is susceptible to capture by the interests of those who participate most actively in it. More governance does not mean better outcomes. It often means worse ones.

The minimum necessary governance for I is: a process for revising protocols; a process for accepting new Instrument definitions; a process for resolving disputes about Host conduct; a record of all governance decisions, publicly available.

Everything else should be governed by the protocols themselves, not by deliberation. A decision encoded in a protocol cannot be captured by any interest group without making a change to the protocol, which must follow declared process, which is a public record.

The goal is governance by architecture, not governance by committee.

### Article 25 · Authority is never inherited

Participation in I, however long, creates no special authority.

The first Host has no more authority than the thousandth. The author of this Constitution has no more authority than any future participant who has read it. The organisation that established the first Instrument has no more authority than any future Instrument author.

Authority in I derives only from: conformance to the protocols (which any party can verify), and the quality of the Observations produced (which is public record).

History creates memory and reputation. Memory and reputation are valuable. They are not authority.

### Article 26 · Responsibility is always personal

While authority in I is never inherited, responsibility is.

A Host that establishes another Host accepts a responsibility of mentorship: to ensure the new Host understands what I requires and has the capacity to meet those requirements.

A Host that ceases operation does not discharge its responsibilities by ceasing. It discharges them by ensuring its Observations have propagated to sufficient other Hosts, by recording its cessation in the host log, and by notifying the Hosts to which it propagated.

Responsibility is personal in the sense that it attaches to the entity that accepted it, not to any institution or successor. If the entity dissolves, the responsibility is not discharged. The host log records what was done and what was not.

---

## Part Four · Instruments

### Article 27 · What makes something an Instrument of I

An Instrument of I is a published, versioned, open protocol specification that has been accepted through the Instrument registration process defined in the governance documents.

To be accepted, an Instrument specification must:

- define a specific, measurable physical quantity or phenomenon
- specify the measurement methodology precisely enough for independent implementation without access to the authors
- define the output format completely and formally
- describe known sources of systematic error and their magnitudes
- specify a calibration procedure that can be performed without specialised equipment not generally available
- include at least one reference implementation and at least one independent validation dataset

A document that meets these requirements and has been accepted through the registration process is an Instrument. A device that implements this document is a realisation of the Instrument. The Instrument and the realisation are different things.

### Article 28 · Instrument 000000

Instrument 000000 is the meta-instrument: the Instrument that defines what an Instrument is.

It produces no Observations of the physical world. Its function is to define the formal properties that all Instruments must have, in a form that is itself an Instrument: structured, versioned, and subject to the same governance as every other Instrument.

Every Instrument in I is formally derived from Instrument 000000. Changes to Instrument 000000 propagate implications to all Instruments. The history of Instrument 000000 is part of the history of every Instrument.

### Article 29 · Instrument versioning

An Instrument version is a complete, self-contained specification. It is not a patch on a previous version. It is a new document that explicitly states its relationship to all previous versions of the same Instrument.

A new version must explicitly state: which previous versions it is compatible with, and why; what has changed from the most recent previous version; what analysis demonstrates the comparability of Observations made under different compatible versions.

Compatibility is never assumed. It is demonstrated.

An Observation references the exact version of the Instrument that produced it. Two Observations made under different versions of an Instrument are comparable only to the extent that the version history documents.

### Article 30 · Instruments cannot be retired

An Instrument that has produced Observations cannot be deleted.

It can be deprecated: marked as superseded, with a recommendation to use a newer version. It can be annotated: with corrections, clarifications, or warnings about known systematic errors discovered after publication. It cannot be removed.

The reason is the same as the reason Observations are immutable. Every Observation references the Instrument that produced it. If the Instrument were removed, the Observation would become uninterpretable: a signal without a specification. The Instrument archive is permanent.

---

## Part Five · Hosts

### Article 31 · What it means to be a Host

To become a Host is to accept a set of responsibilities toward the observational record, toward the network of Hosts, and toward the future.

These responsibilities are operational requirements: to operate Instruments in conformance with their protocols; to record Observations in the canonical format; to sign Observations with the Host's identity key; to propagate Observations to declared peers; to maintain a public operational log; to preserve Raw Data for the duration of the stated availability commitment; to record cessation and propagate remaining Observations before ceasing to operate.

A Host that meets these requirements is a Host. A Host that does not is in breach of the Host Protocol. The breach is recorded in the network's public record. No punishment follows from this Constitution. The record itself is the consequence.

### Article 32 · The equality of Hosts

All Hosts are equal.

This is not an aspiration. It is an architectural constraint.

No governance structure in I may give any Host authority over any other Host by virtue of size, wealth, duration of participation, institutional prestige, geographic location, or political influence.

What differs is the record, which is public and speaks for itself.

### Article 33 · Host lineages

A Host may establish another Host. The establishing Host takes responsibility for ensuring the new Host understands the requirements of I and has the capacity to meet them.

This creates a lineage: a public record of which Hosts established which others. Lineages preserve institutional memory. They record the propagation of practice and understanding across the history of I.

Lineages do not create hierarchy. The new Host owes nothing to the establishing Host beyond what the protocols require of every Host. The establishing Host has no authority over the new Host. The lineage is a historical fact, not a power relation.

### Article 34 · The geographic obligation

The purpose of I — to enable humanity to collectively observe reality — is not fulfilled by a network of Hosts concentrated in wealthy regions.

The phenomena most important to observe are often in the places least served by existing monitoring infrastructure. The geographic distribution of Hosts is therefore not a secondary concern. It is a measure of whether I is doing what it says it is doing.

The network's coverage map is a moral map. Where it is blank, the world is unobserved.

---

## Part Six · Governance

### Article 35 · The purpose of governance in I

Governance in I exists to maintain the integrity of the protocols, to allow I to evolve without losing its identity, and to resolve disputes in a manner consistent with the principles of this Constitution.

Governance in I does not exist to direct the network, allocate resources, rank participants, or represent I to external parties.

### Article 36 · Governance by protocol

The primary mechanism of governance in I is the protocol.

A protocol defines what is valid and what is not. A Host either conforms to the protocol or does not. The conformance is verifiable by any party. No governance body needs to make a judgment.

This is the most important form of governance in I because it is the most resilient: it does not depend on the continued existence of any committee, the good judgment of any individual, or the integrity of any institution. It depends only on the continued availability of the protocol text and the ability of Hosts to read and implement it.

### Article 37 · Protocol change process

Protocols change through a process that is: open — any participant may propose a change; public — all proposals and deliberations are recorded; deliberate — a minimum period for review is required; conservative — backward compatibility is strongly preferred; demonstrated — changes must have running implementations before adoption.

A protocol change that has no implementation is a hypothesis. A protocol change with a running implementation, demonstrated compatibility with the existing observational record, and rough consensus among active participants is a candidate for adoption.

Rough consensus is not unanimous agreement. It is the absence of sustained, principled objection that has not been addressed.

### Article 38 · The constitutional amendment process

This Constitution may be amended.

No part of this Constitution is permanently immune to amendment, because the world changes and understanding grows.

Constitutional amendment requires: a documented proposal with a full statement of reasons; a deliberation period of no less than one year; demonstrated support from Hosts across at least three distinct geographic regions; an explicit statement of what the amendment changes and why the change is consistent with the spirit of I.

Constitutional amendments that would make I depend on any single organisation, any single technology, or any single jurisdiction are not valid amendments. They are attempts to end I.

### Article 39 · What governance must never become

Governance in I must never become: a membership organisation with exclusive authority; a body that can prevent participation by conforming parties; a vehicle for the interests of large or wealthy participants at the expense of small or less wealthy ones; a mechanism for centralising the observational record; a source of revenue for its operators.

If any governance structure in I acquires any of these properties, it has become incompatible with this Constitution. Participants are not required to recognise its decisions.

### Article 40 · Dispute resolution

Disputes between Hosts are resolved by appeal to the protocols.

If a Host believes another Host is in breach of a protocol, it states the breach precisely, with reference to the protocol text, and submits the statement to the public governance record. The accused Host may respond. The community of Hosts may deliberate. The outcome is a public record.

No sanctions follow from this Constitution. The public record is the consequence. Hosts may individually choose to cease propagating with a Host that has been found in repeated breach. This is their right under the Host Protocol. It is not a punishment administered by any authority.

---

## Part Seven · The Constitutional History of I

### Article 41 · This Constitution has a history

This document is Version 1 of the Constitution of I. It was written in 2026. It will be amended. Every version will be preserved in the constitutional archive. The history of this Constitution is part of I.

The history of I does not begin with this document. It begins with the first Observation ever recorded under an I protocol. That Observation is the true founding moment. Documents can be written before there is anything to document. An Observation can only be made in the present tense.

### Article 42 · Version 1 records its own limitations

This Constitution was written at a particular moment in history, by a small number of people, with the knowledge and limitations of that moment.

It will contain errors. It will contain omissions. It will contain principles that seem obvious now and will seem mistaken in fifty years. It will fail to anticipate developments that will seem obvious in fifty years and are unimaginable now.

These are not arguments against writing it. They are arguments for building in the capacity to amend it. The amendment process is not a concession to uncertainty. It is the acknowledgement that a living infrastructure requires a living constitution.

### Article 43 · The invariants

Whatever changes in future versions of this Constitution, the following properties must be preserved.

> **I has no owner.**
> No individual, organisation, government, or any other entity may own I, own the observational record of I, or own the protocols that define I. The observational record is the common heritage of humanity. It may not be privatised, enclosed, or made exclusive in whole or in part, by any party, in any version of this Constitution.

> **Observations are immutable.**
> No version of this Constitution may permit the alteration or deletion of Observations. Observations may be annotated. They may be flagged. They may be contextualised by new knowledge. They may not be changed.

> **The protocols are open.**
> No version of this Constitution may permit the creation of a protocol that any conforming party cannot implement freely, without licence, fee, or permission.

> **All Hosts are equal.**
> No version of this Constitution may create permanent hierarchy among Hosts based on any property other than their record of conduct, which is public, auditable, and the same standard for all.

> **The constitutional history is permanent.**
> No version of this Constitution may permit the deletion of any previous version. The history of I's self-definition is part of I. It may be annotated. It may not be erased.

---

## Part Eight · Closing Articles

### Article 44 · What this Constitution cannot do

This Constitution cannot enforce itself.

No court enforces it. No government backs it. No police protects it. Its authority rests entirely on the willingness of those who implement I to implement it consistently with what this document says.

This is not a weakness. It is the honest description of how all constitutions work in practice. The difference is that most constitutions are backed by state power and this one is not.

The strength of this Constitution is that it describes something that is genuinely valuable to implement correctly: an infrastructure that produces trustworthy, permanent, open records of the world. Parties who implement it incorrectly produce something else. What they produce may be useful. It is not I.

### Article 45 · What this Constitution can do

This Constitution can establish a shared vocabulary.

It can define what counts as an Observation and what does not. What counts as a conforming Host and what does not. What counts as a valid Instrument and what does not. What counts as I and what does not.

By establishing these definitions in a document that is itself part of I's permanent record, this Constitution enables anyone, at any time, to determine whether any particular thing is consistent with what I is.

That is the function of a constitution. Not enforcement, but definition. Not power, but meaning.

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
