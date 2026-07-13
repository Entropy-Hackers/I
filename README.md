# I

This repository hosts the current public definition of I: the Public Constitutional Archive of a living scientific infrastructure.

---

Read the Constitution first. Then read the Manifest. Then read Instrument 000000.

---

## What is I

I is a distributed scientific infrastructure: a set of open protocols, a community of Hosts, a body of Instruments, and an accumulating record of Observations of the world.

An Instrument in I is a published protocol specification — a precise description of what to measure, how, and in what format. Any conforming device, built anywhere, by anyone, is a realisation of that Instrument. Observations are signed, propagated across independent Hosts, and held permanently, so no single failure can destroy the record. The record belongs to everyone.

## Repository structure

```
├── CONSTITUTION.md       — What I is. What cannot change.
├── MANIFEST.md           — Why I exists. What it is trying to do.
├── VOCABULARY.md         — Precise definitions of all terms.
├── DESIGN_PRINCIPLES.md  — Architectural decisions and their reasons.
├── LICENSE               — CC0. No rights reserved.
│
├── protocols/            — Binding technical specifications.
│   ├── IDENT/            — Identity and cryptographic attribution.
│   ├── INSTR/            — Instrument definition and versioning.
│   └── HOST/             — Host obligations and network interface.
│
├── instruments/          — Published instrument specifications.
│   └── 000000/           — Atmospheric particulate. The first instrument.
│
├── hosts/                — Public records of network hosts.
├── observations/         — Index and provenance of the observation record.
├── analyses/             — Reproducible analyses of observation data.
├── knowledge/            — Knowledge claims with full provenance chains.
└── governance/           — How I makes decisions about itself.
```

## How to participate

Participation requires no membership process, no fee, and no approving committee.

Participation means implementing the protocols and contributing to this repository. A Host that operates a conforming Instrument realisation and propagates signed Observations is a Host. A scientist who submits an Instrument definition via pull request is an Instrument author. A contributor who proposes a protocol revision and argues for it publicly is a protocol contributor.

The only credential is the work.

If you are considering participation, start here:

1. Read [`CONSTITUTION.md`](CONSTITUTION.md)
2. Read [`MANIFEST.md`](MANIFEST.md)
3. Read [`instruments/000000/`](instruments/000000/)
4. Open an issue or submit a pull request.

## Licence

CC0. No rights reserved. See [`LICENSE`](LICENSE).

---

*The network begins with the first observation.*
