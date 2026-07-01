# Vocabulary of I

**Version 1 · 2026**

All capitalised uses of these terms throughout I documents refer to the definitions given here. When a term appears capitalised in any I document, it is being used in its I-defined sense, which may differ from its ordinary scientific or technical usage.

When in doubt about the meaning of a term, consult this document first, then the relevant Article in `CONSTITUTION.md`.

---

## Analysis

Any process that takes one or more Observations as input and produces a derived product as output.

An Analysis is reproducible when: its input Observations are precisely identified by their unique IDs; its procedure is specified completely as executable code; its computational environment is described sufficiently that the procedure can be re-executed by any party with access to the input Observations.

An Analysis that cannot be reproduced from its stated inputs is not Analysis in the sense of I. It is assertion.

*See also: Observation, Knowledge, Raw Data.*  
*Defined in: Constitution Article 11.*

---

## Availability Commitment

A Host's public declaration of how long it will retain the Raw Data of Observations it has produced and make them accessible to peers.

An Availability Commitment is not indefinite unless explicitly stated as such. When an Availability Commitment expires or a Host ceases operation, the Host's obligation is to propagate its Observations more widely before ceasing, not to discard them.

*See also: Host, Stewardship, Propagation.*

---

## Calibration Record

A signed document linking an Instrument Realisation to a measurement against known standards, produced at a specific time and by a specific procedure, establishing the Realisation's accuracy at that moment.

Calibration Records are linked to Observations by content hash. They are part of the provenance chain.

*See also: Instrument, Observation, Provenance.*

---

## Constitutional Archive

The public git repository at `github.com/Entropy-Hackers/I`, containing the Constitution, the Manifest, the Vocabulary, the Design Principles, the protocol specifications, the Instrument definitions, the Host records, the observation index, the analyses, the knowledge claims, and the governance records.

The Constitutional Archive is not I. It hosts the current public definition of I.

---

## Continuity

The property of I that ensures its function persists across changes of technology, organisation, funding, and personnel.

Continuity is produced by the architecture — through propagation, protocol publication, constitutional versioning, and Host lineages — not guaranteed by any organisation.

*Defined in: Constitution Article 18.*

---

## Deprecation

The status of an Instrument version that has been superseded by a newer version, marked as no longer recommended for new Observations.

A deprecated Instrument cannot be deleted. Its specification remains in the archive permanently. Observations produced under a deprecated version remain valid and interpretable.

*See also: Instrument, Instrument versioning.*  
*Defined in: Constitution Article 30.*

---

## Host

Any entity that operates one or more Instrument Realisations, records the resulting Observations, propagates those Observations according to the propagation protocol, and accepts the responsibilities defined in the Host Protocol.

A Host may be an individual, a family, a school, a laboratory, a university, a company, a city, a research institute, or any other entity capable of sustained responsible operation. All Hosts are equal in authority within I regardless of size, wealth, or duration of participation.

*See also: Host Protocol, Propagation, Stewardship, Identity.*  
*Defined in: Constitution Article 9.*

---

## Host Lineage

The historical record of which Host established which other Hosts.

A lineage preserves institutional memory and records the propagation of practice and understanding across the history of I. It does not create hierarchy or authority. The new Host owes nothing to the establishing Host beyond what the protocols require of every Host.

*Defined in: Constitution Article 33.*

---

## Host Protocol

The binding technical specification defining Host obligations: operating Instruments in conformance with their protocols; recording Observations in the canonical format; signing Observations; propagating to at least two peer Hosts; maintaining a public operational log; preserving Raw Data for the stated Availability Commitment; recording cessation.

*Location in repository: `protocols/HOST/`*

---

## Identity

A cryptographic public/private key pair held by every participant in I — every Host, every Instrument author, every contributor.

The public key is the identity. It is globally unique, self-generated, and requires no issuing authority. All Observations are signed by the Identity of the Host that produced them. Identity authenticates actions, not persons.

*Defined in: Constitution Article 10.*

---

## Instrument

A protocol that specifies how a class of Observations is to be produced: the physical quantity or phenomenon to be measured; the method of measurement; the conditions of validity; the output format; the calibration procedure; the known sources of systematic error.

An Instrument is a document. The document is the Instrument. Hardware that implements the document is a Realisation. An Instrument is not hardware.

*See also: Instrument 000000, Instrument Realisation, Instrument versioning, Raw Data.*  
*Defined in: Constitution Article 8.*

---

## Instrument 000000

The meta-instrument: the Instrument that defines what an Instrument is.

Instrument 000000 produces no Observations of the physical world. Its function is to define the formal properties that all Instruments must have. Every Instrument in I is formally derived from Instrument 000000.

*Location in repository: `instruments/000000/`*  
*Defined in: Constitution Article 28.*

---

## Instrument Protocol

The binding technical specification defining how Instruments are specified, versioned, and referenced: the required fields, the versioning rules, the compatibility statement requirements, the signing requirements.

*Location in repository: `protocols/INSTR/`*

---

## Instrument Realisation

A physical device or software system that implements a specific version of an Instrument specification and produces conforming Observations.

A Realisation is not the Instrument. The Instrument is the specification. Many Realisations may implement the same Instrument. When a Realisation fails, the Instrument continues.

---

## Knowledge

A structured claim about the world supported by one or more Analyses, which are in turn supported by one or more Observations, which are in turn produced by one or more Instruments.

A Knowledge claim with no traceable chain to Observations is not Knowledge in the sense of I. It is opinion.

Knowledge claims can be disputed, revised, extended, and superseded. When they are, the revision and its basis are recorded alongside the original claim. Neither is deleted.

*See also: Analysis, Observation, Provenance.*  
*Defined in: Constitution Article 12.*

---

## Memory

The accumulated body of Observations in I.

Memory grows continuously. Memory never diminishes: Observations are immutable and permanent. Memory is distributed across all Hosts. Memory is the purpose of I materialised.

*Defined in: Constitution Article 16.*

---

## Observation

A record of a measurement made by a conforming Instrument at a specific location and time, in accordance with the Instrument's protocol.

An Observation is singular, immutable, signed, and attributed (to a specific Instrument version and Host). An Observation that has been altered is not an Observation. It is a fabrication.

*See also: Raw Data, Instrument, Host, Identity, Propagation.*  
*Defined in: Constitution Article 6.*

---

## Operational Log

A Host's public, continuously updated record of its operational status: periods of operation, gaps in observation, calibration events, instrument changes, and cessation.

The Operational Log is part of the Host's public record and contributes to its reputation.

---

## Protocol

A complete, public specification of a procedure that any conforming party can implement independently, producing results comparable to those of any other conforming party.

A Protocol is defined by its text. No licence, fee, or permission is required to implement a Protocol of I. When a Protocol and an implementation conflict, the Protocol is authoritative.

*Defined in: Constitution Article 13.*

---

## Propagation

The mechanism by which Observations spread across the network of Hosts without passing through any centre.

Propagation is a protocol obligation, not a courtesy. A Host that does not propagate Observations to its declared peers is in breach of the Host Protocol.

*See also: Host Protocol, Memory, Continuity.*  
*Defined in: Constitution Article 14.*

---

## Provenance

The complete, auditable chain connecting a Knowledge claim back through the Analyses that support it, through the Observations on which those Analyses operated, to the Instrument versions and Hosts that produced those Observations.

Provenance is embedded in Observations (through signing and attribution) and in Analyses (through precise identification of input Observations). A claim whose provenance cannot be traced is not Knowledge in the sense of I.

---

## Raw Data

The unmodified output of a sensor or measurement process as received from the physical world, prior to any transformation.

Raw Data is immutable within an Observation. No quality control, averaging, calibration correction, or interpolation is applied to Raw Data before it becomes part of an Observation. These operations belong to Analysis.

*Defined in: Constitution Article 7.*

---

## Realisation

See *Instrument Realisation*.

---

## Stewardship

The disposition of a Host toward its Observations: the obligation to preserve, propagate, and hand over, rather than the right to destroy, withhold, or sell.

Stewardship is the ethical disposition that holds the network together when no other obligation does.

*Defined in: Constitution Article 15.*

---

## Trust

In I, trust is produced by the architecture, not claimed by the participants.

The cryptographic signature on an Observation does not require trust in the Host. It requires only the ability to verify the signature. The reproducibility requirement on Analysis does not require trust in the analyst. It requires only the ability to re-run the procedure. The public constitutional archive does not require trust in its maintainers. It requires only the ability to read the history.

*Defined in: Constitution Article 23.*

---

*Vocabulary of I · Version 1 · 2026 · CC0 · github.com/Entropy-Hackers/I*
