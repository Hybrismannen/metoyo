# METOYO — Repository Status

**Snapshot:** 2026-09-23  
**Repository:** `Hybrismannen/metoyo`

## Status board

| Domain | Status | Canonical file |
|---|---|---|
| Public identity / naming | ✅ Defined | `docs/00-canonical-identity.md` |
| System flow | ✅ Defined | `docs/01-system-model.md` |
| Gift Whisperer / Trident | ✅ Defined | `docs/02-ritual-engine.md` |
| 20-persona canon | ✅ Defined | `docs/03-persona-canon.md` |
| Gesture grammar | ✅ Defined | `docs/04-gesture-grammar.md` |
| Spatial Memory Architecture | ✅ Defined | `docs/05-spatial-memory.md` |
| Reflection Chamber | ✅ Defined | `docs/06-reflection-chamber.md` |
| Ethics/privacy/governance | ✅ Defined | `docs/07-ethics-privacy-governance.md` |
| Technical architecture | ✅ Defined at system level | `docs/08-technical-architecture.md` |
| Strategy/evaluation | ✅ Consolidated | `docs/09-strategy-roadmap-evaluation.md` |
| Collaboration/funding/sourcing | ✅ Consolidated | `docs/10-collaboration-funding-sourcing.md` |
| Pius lineage | ✅ Boundaried | `docs/11-pius-lineage.md` |
| Editorial/source protocol | ✅ Defined | `docs/12-editorial-source-protocol.md` |
| Design language | ✅ Defined | `docs/13-design-language.md` |
| Persona registry | ✅ Machine-readable | `data/personas.yaml` |
| Gesture registry | ✅ Machine-readable | `data/gesture-grammar.yaml` |
| Trident schema | ✅ Machine-readable | `data/trident-schema.yaml` |
| Historical source extracts | ✅ Archived | `archive/source-extracts/` |
| Contribution rules | ✅ Defined | `CONTRIBUTING.md` |
| Decision log | ✅ Defined | `DECISIONS.md` |
| Development history | ✅ Defined | `HISTORY.md` |
| Source inventory | ✅ Defined | `SOURCE_INDEX.md` |
| License posture | ✅ Defined | `LICENSE.md` |

## What is deliberately not locked yet

The repository does **not** currently declare these implementation choices canonical:

- frontend framework;
- model provider;
- database;
- analytics provider;
- hosting;
- exact account/persistence model;
- exact source-search provider;
- payment or commercial architecture;
- activated governance body;
- current funding application;
- current launch date.

Those require new decisions, not automatic inheritance from 2025 planning.

## Next implementation gate

Before code build, resolve:

1. target deployment surface;
2. model/provider privacy contract;
3. persistence/no-persistence implementation;
4. source/local-business lookup approach;
5. consent and reflection storage behavior;
6. accessibility baseline;
7. localization starting languages;
8. whether source documents/binary decks will also be committed as binary artifacts.

The conceptual system itself is now consolidated enough for implementation design.
