# Version and Freeze Protocol

## Version

Target: **METOYO 1.0**

This branch is a design candidate and must not be described as production 1.0 until frozen.

## State progression

```
AUDITED
→ DESIGN-CANDIDATE
→ HUMAN-REVIEWED
→ HUMAN-FROZEN
→ LOVABLE-IMPLEMENTING
→ IMPLEMENTED
→ QA-CLEARED
→ RELEASE-CANDIDATE
→ PUBLIC
```

No state may be skipped in repository metadata.

## Freeze manifest

At HUMAN-FROZEN, record:

- commit SHA;
- date;
- Human Decision Register state;
- ontology schema version;
- prompt contract version;
- privacy contract version;
- design-token version;
- acceptance-test version;
- source-claim register version.

## Change classes

### Class A — editorial
Copy and non-semantic wording. May be changed without architecture review if meaning is unchanged.

### Class B — interaction
Layout, sequencing or component behavior that does not alter ontology/privacy. Requires UX review.

### Class C — contract
Schema, state machine, prompt output or service interface change. Requires architecture review.

### Class D — canon
Ontology, persona identity, Trident semantics, safety, retention, evidence claim or governance change. Requires explicit human ratification.

Lovable may autonomously implement A/B within defined specifications. It may not originate C/D changes.
