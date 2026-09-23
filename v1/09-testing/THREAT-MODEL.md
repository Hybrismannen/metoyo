# Threat Model

## Protected assets
- raw memory fragments;
- saved rituals;
- reflections;
- user identity;
- optional place context;
- API/provider secrets;
- canonical product contracts.

## Threats

### T1 — Accidental retention
Raw memory logged or stored by app/provider.

Control:
- session-default design;
- log redaction;
- provider configuration review;
- privacy tests.

### T2 — Cross-user data access
Saved ritual exposed through weak authorization.

Control:
- RLS;
- ownership policies;
- deny tests.

### T3 — Prompt injection through user input
Memory text attempts to override system/product policy.

Control:
- hierarchy-separated prompt assembly;
- schema validation;
- safety validation;
- treat user text as data.

### T4 — Recipient profiling creep
Feature expansion turns memories into persistent person dossiers.

Control:
- no recipient entity required in guest core;
- Save Ritual stores a ritual artifact, not a behavioral profile.

### T5 — Source commercialization drift
Affiliate incentives alter suggestions.

Control:
- SourceAdapter policy;
- sponsorship requires explicit governance change/disclosure.

### T6 — Location misuse
Precise recipient location becomes trackable.

Control:
- coarse optional input;
- no passive recipient location;
- no exact address for ideation.

### T7 — Unsafe ritual suggestion
Model suggests trespass/coercion/no-contact circumvention.

Control:
- boundary profiles;
- validator;
- adversarial fixtures.

### T8 — Canon drift by AI builder
Lovable rewrites ontology to make implementation easier.

Control:
- DO-NOT-CHANGE;
- human decision register;
- PR review against v1 contracts.

### T9 — Privacy-copy mismatch
Marketing says “stores nothing” while infrastructure retains data.

Control:
- deployment-derived privacy review before release;
- acceptance test.

## Residual-risk rule

When a privacy/safety guarantee cannot be technically verified, public copy must state the narrower verified behavior.
