# Interaction State Machine

## Canonical states

```
ARRIVAL
  ↓
RELATIONSHIP
  ↓
MEMORY
  ↓
CONTEXT_OPTIONAL
  ↓
READY
  ↓
GENERATING
  ├── ERROR_RECOVERABLE
  └── TRIDENT
         ├── REFINE → GENERATING
         ├── KEEP → COMPLETE
         ├── EXPORT → COMPLETE
         ├── SAVE_GATE → AUTH_OPTIONAL → SAVED → COMPLETE
         └── RESTART → RELATIONSHIP

COMPLETE
  └── REFLECTION_OPTIONAL
```

## State constraints

### ARRIVAL
No tracking prerequisite. No account.

### RELATIONSHIP
Requires exactly one persona ID or a neutral “someone not listed” path.

### MEMORY
Minimum meaningful input is not character count. UI suggests 3–5 fragments but the engine may proceed with fewer if sufficient.

### CONTEXT_OPTIONAL
All fields skippable.

### READY
Client assembles a request object. Raw memory remains session-local unless request transmission to the AI service is required.

### GENERATING
- disable duplicate submissions;
- show restrained loading state;
- no fake progress percentages;
- support cancellation where technically possible.

### TRIDENT
Must validate complete Gift/Source/Ritual structure before rendering.

### SAVE_GATE
Must present what will be stored before authentication/persistence.

### COMPLETE
Core session is successful even with no save.

## Error states

- NETWORK_ERROR
- MODEL_ERROR
- VALIDATION_ERROR
- SOURCE_LOOKUP_ERROR
- SAFETY_REFRAME
- RATE_LIMIT
- SESSION_EXPIRED

Each error must preserve already-entered session state locally where possible without silently persisting it server-side.

## Forbidden transitions

- ARRIVAL → AUTH_REQUIRED
- MEMORY → PERSISTED without consent
- TRIDENT → PURCHASE checkout as default
- COMPLETE → mandatory reflection
- COMPLETE → mandatory share
- ERROR → generic invented Trident
