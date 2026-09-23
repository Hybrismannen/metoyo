# Service Boundaries

## Architecture

```
UI / Session
   |
   v
Ritual Orchestrator
   |---- ModelAdapter
   |---- SourceAdapter
   |---- SpatialAdapter
   |---- PersistenceAdapter (optional)
   |---- TelemetryAdapter (optional/off)
```

## ModelAdapter

Responsibilities:
- structured generation;
- timeout/retry policy;
- provider mapping.

Forbidden:
- persistence decisions;
- analytics;
- persona taxonomy mutation.

## SourceAdapter

Responsibilities:
- local/source category guidance;
- optional concrete source lookup.

Rules:
- no affiliate preference by default;
- label sponsored/commercial relationships if ever introduced;
- source failure must not destroy Gift/Ritual meaning.

## SpatialAdapter

Responsibilities:
- geocoding or place interpretation when explicitly requested.

Rules:
- coarse by default;
- no passive location collection;
- no recipient tracking.

## PersistenceAdapter

Optional.

Required API:
```ts
saveRitual()
listRituals()
getRitual()
deleteRitual()
exportRitual()
```

No persistence call exists on the core generation path unless explicitly invoked.

## TelemetryAdapter

Optional, feature-flagged OFF until HD-002.

Must expose event allowlist. Arbitrary event payloads are forbidden.

## Secrets

All provider secrets stay server-side.

No model key, service-role key or privileged token may be shipped to the browser.

## Backend implementation

Lovable currently supports both Lovable-managed cloud backends and external Supabase-style backends. METOYO therefore treats backend selection as a deployment decision, not domain architecture.

If Supabase is selected:
- RLS enabled on every exposed table;
- grants/policies reviewed per operation;
- RLS tests required before launch;
- service-role access only in trusted server functions.
