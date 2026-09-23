# Lovable Build Sequence

The build is intentionally staged to prevent prompt-driven architecture drift.

## WP0 — Repository intake
- connect Lovable to the METOYO repository/implementation branch;
- ingest `v1/`;
- create a short implementation map;
- no product changes.

Gate: architecture summary matches source contracts.

## WP1 — Foundations
- React/TypeScript/Tailwind project;
- token layer;
- routing;
- semantic shell;
- error boundary;
- accessibility primitives;
- test framework.

Gate: no backend needed.

## WP2 — Static ritual UX
Build screens S00–S03 with local state:
- landing;
- relationship;
- memory;
- optional context.

Gate: complete keyboard/mobile flow.

## WP3 — Trident domain layer
- typed request/response schemas;
- state machine;
- mock ModelAdapter;
- Trident renderer;
- refine behavior;
- validation.

Gate: works entirely with fixtures.

## WP4 — Server AI adapter
- server-side generation endpoint/function;
- provider secret;
- prompt compiler;
- structured response parser;
- one repair pass;
- safe error handling.

Gate: no database required.

## WP5 — Source/spatial adapters
- optional source routing;
- optional coarse spatial input;
- degraded-mode behavior.

Gate: Source failure never destroys Gift/Ritual.

## WP6 — Privacy implementation
- session-only default;
- privacy page derived from actual configuration;
- verify no hidden persistence;
- verify logs.

Gate: guest path creates no application persistence record.

## WP7 — Optional persistence
Only after HD-003/004/005:
- auth;
- Save Gate;
- saved ritual tables;
- RLS;
- delete/export;
- reflection persistence.

Gate: RLS tests pass.

## WP8 — Evaluation/telemetry
Only after HD-002:
- allowlisted minimal events;
- no raw memory payload;
- consent where required.

Gate: ritual works identically with telemetry disabled.

## WP9 — Visual refinement
- motion;
- imagery;
- microcopy;
- responsive polish;
- reduced motion;
- accessibility audit.

## WP10 — Adversarial/ritual QA
Run:
- unsafe relationship cases;
- no-contact scenario;
- minors;
- workplace power;
- invented-preference tests;
- generic-output tests;
- provider outage;
- source outage;
- privacy tests.

## WP11 — Release candidate
- pin versions;
- build;
- security scan;
- acceptance suite;
- human visual/product review;
- freeze release SHA.

No public publish before WP11 gate.
