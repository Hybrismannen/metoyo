# Data Lifecycle

**Status:** design contract; persistence details depend on HD-003/HD-004/HD-005.

## Data classes

### D0 — Static public content
Examples:
- persona definitions;
- gesture grammar;
- product copy.

Retention: repository/deployment lifecycle.

### D1 — Ephemeral ritual input
Examples:
- memory fragments;
- selected persona;
- optional context;
- refinement.

Default:
- client/session state;
- sent to server/model only to generate requested output;
- not written to persistent application tables.

### D2 — Generated ritual
Gift / Source / Ritual response.

Default:
- session-local;
- export/copy allowed;
- persistence only through Save Gate.

### D3 — User-saved ritual
Exists only after explicit save.

Must carry:
- owner ID;
- created time;
- schema version;
- fields chosen for storage.

Must support delete/export.

### D4 — Reflection
Private by default.
Persistence only if user chooses to save.

### D5 — Operational telemetry
Examples:
- request success/failure;
- latency;
- provider error category.

Must not contain raw memory fragments unless a separately authorized debugging procedure explicitly requires it.

## Default lifecycle

```
input
→ transient client state
→ transient server processing
→ model processing
→ structured response
→ session
→ discard
```

No database write is required for the core ritual.

## Save lifecycle

```
session result
→ user chooses Save
→ disclosure
→ authentication if required
→ explicit confirmation
→ minimal persisted record
```

## Deletion

Deleting a saved ritual must remove:
- application row;
- linked reflection;
- related user-owned attachments if implemented.

Deletion policy must state any provider backup limitations truthfully.

## Sensitive content

Memory fragments can contain intimate personal information even when not formally categorized as special-category data. The system therefore treats them as high-sensitivity user content operationally.

## Provider disclosure

Public privacy copy must identify:
- whether a model provider processes content;
- whether content is retained by that provider;
- deployment region where material;
- any operational logging.

The copy must be generated from actual configuration, not aspiration.
