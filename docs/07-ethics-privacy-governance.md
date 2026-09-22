# 07 — Ethics, Privacy & Governance

## 1. Ethical posture

METOYO is designed around **relational integrity, data minimization, voluntary use, poetic restraint, and system disappearance**.

The ethical commitment is architectural. It must be visible in:
- data flows;
- interface choices;
- model prompts;
- analytics;
- contributor agreements;
- governance;
- sourcing;
- future business decisions.

## 2. Forget-by-default

The canonical default is:

> **Do not retain relationship data merely because retention is technically convenient.**

User inputs such as:
- memory clusters;
- recipient references;
- relational personas;
- spatial cues;
- Trident outputs;
- reflections;

should be ephemeral unless a user deliberately chooses to save something.

## 3. No relational profiling

METOYO should not create hidden recipient or relationship profiles.

Disallowed default patterns include:
- persistent "people" records;
- inferred personality traits;
- sentiment scoring of relationships;
- gift history used for recommendation optimization;
- embeddings retained to reconstruct private memory;
- ad targeting;
- cross-session behavioral profiling.

## 4. Data categories

### Ephemeral operational data
Used only to generate the current interaction.

### Technical logs
Only what is necessary for security/reliability. Historical contributor agreements proposed anonymization and deletion within **14 days** for debugging logs. Any implementation should minimize further where feasible.

### User-saved artifacts
Created only by explicit user action and controlled by the user.

### Voluntary research/project feedback
Must be clearly separated from private ritual data and consented independently.

## 5. Model-data rule

Project source agreements state that user prompt inputs/outputs are not to be reused to train external or proprietary systems.

Implementation choices must therefore be assessed for:
- model provider retention;
- training defaults;
- API data-use terms;
- logs;
- observability tools;
- third-party processors.

Do not make privacy claims that the actual technical stack cannot support.

## 6. Consent

Consent should be:
- specific;
- understandable;
- revocable where relevant;
- independent of core access where possible.

Especially separate consent for:
- saving reflections;
- public story submission;
- analytics beyond essential service operation;
- exact location;
- contact/reminders;
- research participation.

## 7. Emotional boundaries

METOYO should not automate emotionally high-stakes decisions.

Special caution is required for:
- grief;
- trauma;
- estrangement;
- apology;
- reconciliation;
- forgiveness;
- abuse dynamics;
- workplace power;
- minors;
- former intimate relationships.

The engine may support reflective wording or low-intensity gesture ideation, but should not tell a user what another person feels, owes, wants, or will forgive.

## 8. Non-coercive UX

Disallowed design patterns:
- countdown pressure;
- fake scarcity;
- social proof pressure;
- streaks;
- compulsory reflection;
- guilt notifications;
- manipulative defaults;
- emotional scoring;
- rewards for disclosure;
- recommendations framed as morally superior.

## 9. Commons and licensing

Historical project materials are framed under **CC BY-NC-SA 4.0**.

Contributor agreements established principles that:
- contributors receive attribution;
- portfolio use is allowed under the license;
- independent commercialization requires explicit alignment/permission;
- the non-commercial and share-alike posture should remain visible.

This repository's `LICENSE.md` records the project license posture. Individual third-party assets may have separate licenses and must be handled accordingly.

## 10. Contributor ethics

Contributors can include:
- developers;
- UX designers;
- prompt engineers;
- privacy/legal advisors;
- writers/editors;
- illustrators/symbol designers;
- systems architects.

All contributors should understand:
- the public/internal naming distinction;
- forget-by-default architecture;
- non-surveillance design;
- tone integrity;
- boundary rules;
- provenance and versioning.

## 11. Governance model

Historical materials envisioned stewardship rather than conventional ownership rhetoric, including a possible rotating review group ("Whisper Circle").

A future governance body could review:
- prompt changes;
- new personas;
- gesture grammar additions;
- localization;
- public story submissions;
- privacy-impact changes;
- research protocols.

No governance structure is considered active merely because it appeared in planning documents. Activation requires explicit versioned adoption.

## 12. Release gate

Before a meaningful release, ask:

### Room
Does the change create room or consume it?

### Data
Does it add retention, inference, or third-party exposure?

### Relational sovereignty
Does it preserve human judgment?

### Boundary
Could the ritual become intrusive?

### Commercial pressure
Does revenue logic distort the system's purpose?

### Provenance
Can we trace the change to a documented decision?

### Reversibility
Can a user decline, delete, or opt out?

## 13. Core rule

> Care is not something the system is allowed to extract in order to prove that it created care.

Ethics in METOYO is not a compliance layer after design. It is part of the form of the system.
