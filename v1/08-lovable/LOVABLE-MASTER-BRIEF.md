# Lovable Master Brief — METOYO 1.0

**DO NOT EXECUTE UNTIL THE BRANCH IS HUMAN-FROZEN.**

## Mission

Implement METOYO 1.0 as a production-quality ritual web application from the contracts in `v1/`.

Lovable is permitted to write implementation code. Lovable is not permitted to redefine the product ontology.

## Current platform target

Use Lovable's modern standard web stack:
- React;
- TypeScript;
- Tailwind;
- GitHub synchronization;
- server-side functions/backend through the selected deployment profile.

Supabase-compatible persistence may be used only for optional user-owned saved data and server functions. Core ritual use must work without a user account and without persistent ritual tables.

## Source-of-truth order

1. RATIFIED entries in `00-governance/HUMAN-DECISION-REGISTER.md`
2. `02-ontology/*.yaml`
3. product/UX/privacy/AI contracts in `v1/`
4. canonical repository docs
5. historical archive

Do not infer product behavior from archive material when v1 contracts exist.

## Build requirements

### Public core
- landing;
- relationship/persona selection;
- memory fragment input;
- optional context;
- generation;
- Trident result;
- refinement;
- complete/export;
- privacy/about/accessibility.

### Optional modules
- Save Ritual;
- authentication;
- My Rituals;
- reflection persistence.

These remain behind feature/config gates until relevant human decisions are ratified.

## Architectural constraints

- Domain logic outside page components.
- Provider clients behind adapters.
- No privileged keys in browser code.
- No raw arbitrary telemetry payloads.
- No database write on the default guest generation path.
- AI generation server-side.
- Output validated against a typed Trident schema before render.
- errors never create fabricated fallback content.
- persona constellation must not drive runtime logic while HD-001 is unresolved.

## UI direction

Quiet editorial ritual:
- warm paper field;
- strong typography;
- generous whitespace;
- light translucent surfaces;
- restrained motion;
- no dashboard aesthetic;
- mobile-first;
- WCAG 2.2 AA target.

Use `04-design-system/TOKENS.md` as the starting token contract.

## Quality bar

This is not a throwaway MVP.

Every state must have:
- loading;
- success;
- empty;
- validation;
- recoverable error;
- keyboard behavior;
- mobile behavior;
- reduced-motion behavior.

## Security

If Supabase is selected:
- RLS on every exposed table;
- least-privilege grants;
- operation-specific policies;
- database tests for anon/authenticated allow + deny behavior;
- service-role key only in trusted server functions.

Run Lovable's available security checks before publish, but do not treat a platform scan as a substitute for the METOYO acceptance tests.

## Completion definition

Implementation is complete only when `ACCEPTANCE-TESTS.md` passes and no DO-NOT-CHANGE invariant has been altered.
