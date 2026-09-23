# API Contracts

## POST /api/ritual/generate

Request:
```json
{
  "schemaVersion": "1.0",
  "personaId": "mentor",
  "memoryFragments": ["chalk dust", "spiral notebook", "thesis night"],
  "context": {
    "tone": "quiet",
    "budgetBand": "low",
    "diyOpenness": "high"
  },
  "refinementMode": null
}
```

Response:
```json
{
  "schemaVersion": "1.0",
  "gift": {
    "title": "The Margin Notebook",
    "form": "hand-bound notebook",
    "meaning": "..."
  },
  "source": {
    "routeType": "make_or_local",
    "guidance": "..."
  },
  "ritual": {
    "modeId": "silent_exchange",
    "action": "...",
    "wording": "..."
  },
  "rationale": {
    "memoryLinks": ["chalk dust", "spiral notebook"]
  },
  "safety": {
    "status": "clear"
  }
}
```

## Error envelope

```json
{
  "error": {
    "code": "MODEL_UNAVAILABLE",
    "retryable": true,
    "message": "The ritual could not be formed right now."
  }
}
```

## POST /api/ritual/refine

Same request identity plus:
- prior Trident;
- refinement mode.

The server may regenerate from normalized inputs; it must not require a persisted session.

## Save endpoints

Only active when optional persistence is enabled:

- POST /api/rituals
- GET /api/rituals
- GET /api/rituals/:id
- DELETE /api/rituals/:id
- GET /api/rituals/:id/export

Authentication is required for user-owned persistence.

## Contract rule

All external/provider-specific payloads are normalized behind server interfaces. The browser consumes METOYO contracts only.
