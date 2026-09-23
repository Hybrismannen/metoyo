# METOYO 1.0 — Pre-Lovable Design Baseline

**Status:** DESIGN CANDIDATE — NOT YET HUMAN-FROZEN  
**Branch:** `design/metoyo-1.0-pre-lovable`  
**Audit ancestor:** `audits/2026-09-23-metoyo-lifetime-audit/`

This directory defines the future-state METOYO 1.0 architecture that is to be frozen before production implementation in Lovable.

## Governing principle

Lovable is an implementation environment, not the source of product ontology.

The implementation must preserve:

```
METOYO
  public-facing ritual space / condition
      ↓
The Gift Whisperer
  internal orchestration engine
      ↓
Memory → Relationship → Prompt → Trident → Human Judgment → Gesture
                                      ↓
                              optional reflection
```

## Design rules

1. Stable source-backed ritual logic may be frozen.
2. Audit conflicts remain explicit until human-ratified.
3. Historical vendor choices do not silently become present dependencies.
4. Guest use is the primary path.
5. Persistence is optional, explicit and separable.
6. Human judgment is a required gate before a suggestion becomes a real-world act.
7. Safety is architectural, not merely prompt wording.
8. The system must be able to become less necessary to the user.
9. AI implementation freedom is bounded by written contracts.
10. Lovable must not modify ontology, privacy, prompt policy or data contracts on its own.

## Directory

- `00-governance/` — authority, decisions, freeze rules
- `01-product/` — product definition, journeys and state machine
- `02-ontology/` — canonical machine-readable domain model
- `03-ux/` — information architecture and screen contracts
- `04-design-system/` — visual tokens and component grammar
- `05-ai/` — Gift Whisperer orchestration and prompt contracts
- `06-data-privacy/` — data lifecycle, consent and measurement
- `07-services/` — provider and service boundaries
- `08-lovable/` — bounded implementation handoff
- `09-testing/` — acceptance, safety and regression tests
- `10-research/` — claims and evidence state

## Freeze condition

METOYO 1.0 may be marked **HUMAN-FROZEN** only when every `BLOCKING` decision in the Human Decision Register has an explicit decision and author/date trace.

Until then, Lovable may be used only against explicitly non-blocked contracts or in a disposable prototype environment.
