# Human Decision Register

This register exists to prevent assistant inference from becoming human canon.

## Status vocabulary

- **RATIFIED** — explicit human decision exists.
- **SOURCE-STABLE** — repeated direct project sources agree; no current contradiction.
- **PROPOSED DEFAULT** — implementation-ready proposal awaiting human ratification.
- **PENDING** — cannot be represented as settled.
- **RETIRED** — superseded by explicit human decision.

## Register

| ID | Decision | Status | Proposed/default position | Build dependency |
|---|---|---|---|---|
| HD-001 | Persona constellation placement of **Self / Boss / Muse** | PENDING | Keep personas operational, mark disputed constellation metadata unresolved; runtime does not branch on constellation | Non-blocking for engine; blocking for final persona browsing IA |
| HD-002 | Analytics doctrine | PROPOSED DEFAULT | No third-party behavioral analytics in v1. Operational aggregate telemetry only if separately ratified and non-identifying | Blocking for production telemetry |
| HD-003 | Backend ownership | PROPOSED DEFAULT | Provider abstraction; production preference = project-controlled Supabase rather than provider-locked persistence | Blocking for deployment, not UI build |
| HD-004 | Optional account / Save Ritual | PROPOSED DEFAULT | No account required. Save is optional, off by default and separately consented | Blocking for persistence implementation |
| HD-005 | Reflection storage duration | PROPOSED DEFAULT | Session-only unless user explicitly saves; user-owned records deletable/exportable | Blocking for persistence implementation |
| HD-006 | Location precision | PROPOSED DEFAULT | Coarse place input by default; exact addresses never requested for ideation | Non-blocking |
| HD-007 | Source routing / commerce | PROPOSED DEFAULT | Source is access guidance, not affiliate or marketplace ranking | Non-blocking |
| HD-008 | Software license | PENDING | Documentation remains CC BY-NC-SA posture; executable code requires explicit license | Blocking before public code release |
| HD-009 | Public launch languages | PROPOSED DEFAULT | Swedish + English architecture-ready; copy may launch one language first | Non-blocking for architecture |
| HD-010 | Current masterplan authority | PENDING | v8 remains evidence, not latest-canon claim, until referenced v9 is found or retired | Blocking for historical baseline only |
| HD-011 | HCC / Pius formal clearance label | PENDING | Do not claim Seal of Accord until an explicit clearance artifact exists | Blocking for any public Pius-clearance claim |
| HD-012 | Visual identity final approval | PROPOSED DEFAULT | Quiet editorial/tactile system defined in design tokens; final visual freeze requires human approval | Blocking for final launch polish |

## Already stable

The following do not require a new decision to continue design:

- METOYO is public-facing.
- Gift Whisperer is the internal execution engine.
- Memory precedes object.
- relationship informs logic.
- Trident = Gift / Source / Ritual.
- Gesture Grammar exists as six canonical modes.
- Reflection is optional.
- Spatial memory is optional.
- no coercive urgency, streaks or growth-hacking mechanics.
- user judgment remains final.
- system disappearance / declining dependency can be a positive outcome.

## Ratification format

Every human decision should be recorded as:

```yaml
id: HD-###
decision: ...
selected: ...
ratified_by: human
ratified_at: YYYY-MM-DD
supersedes: [optional IDs]
notes: ...
```

Assistant-generated text may prepare a proposed value but must never populate `ratified_by: human` without an explicit user decision.
