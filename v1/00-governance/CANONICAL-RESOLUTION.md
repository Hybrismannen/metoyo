# Canonical Resolution Layer

## Purpose

The audit identified a distinction the previous repository did not enforce strongly enough:

1. historical source,
2. assistant-derived synthesis,
3. human-ratified canon.

METOYO 1.0 makes this separation structural.

## Canonical precedence

For implementation:

1. explicit Human Decision Register entry marked RATIFIED;
2. SOURCE-STABLE METOYO 1.0 contract;
3. current v1 machine-readable ontology;
4. canonical source-backed documentation;
5. historical sources;
6. archive material;
7. assistant inference.

A lower layer cannot override a higher layer.

## Conflict handling

If Lovable, a model provider, contributor or future automation encounters conflict:

```
STOP affected behavior
→ identify contract
→ record conflict
→ preserve user data
→ fall back to safest non-persistent behavior
→ require human resolution for ontology/policy changes
```

It must not choose a new product rule through implementation convenience.

## Resolution of audit findings for design purposes

### Source archive truncation
Treated as a provenance defect, not a product-logic dependency. No v1 contract may cite the truncated GitHub copy as sole evidence when the original project artifact is available.

### Persona taxonomy conflict
Persona identity and prompt logic remain usable. Constellation is metadata, not an execution key. Disputed assignments remain unresolved until HD-001.

### Privacy / analytics conflict
The v1 architecture makes telemetry optional and physically separate from ritual operation. The ritual works with telemetry disabled.

### Vendor stack conflict
Carrd, Airtable, GA4, Bitly, Zapier, Typeform/Tally, Looker and earlier model names are historical implementation proposals. Their functions are preserved through interfaces; their vendor identities are not mandatory runtime canon.

### Pius lineage
Pius explains development lineage and audit method. METOYO must not claim formal Pius/HCC clearance unless an explicit clearance artifact exists.

## Frozen boundaries

Lovable may not autonomously change:

- brand/engine relationship;
- Trident semantics;
- memory-first flow;
- privacy defaults;
- safety rules;
- persona identities;
- Gesture Grammar semantics;
- data retention policy;
- human decision status;
- claims/evidence state.

Those are governance-bound.
