# 05 — Spatial Memory Architecture

## 1. Premise

Gifts have origin.

A place can carry memory, effort, cultural meaning, practical context, or narrative continuity. METOYO therefore allows geography to influence the **Source** and **Ritual** branches of the Trident without turning location into a surveillance layer.

This is the **Spatial Memory Architecture**.

## 2. Three optional spatial inputs

The system may ask:

1. **Where are you now?**
2. **Where are they?**
3. **Where should this gift feel like it came from?**

These fields are optional.

| Input | Function | Ritual meaning |
|---|---|---|
| Giver place | logistical/contextual grounding | "this is where I am acting from" |
| Recipient place | accessibility and local fit | "this enters their world" |
| Symbolic origin | narrative provenance | "this comes from somewhere meaningful" |

## 3. Symbolic origin

The third field is not the same as delivery location.

A user may want a gift to carry meaning from:
- a hometown;
- a city where the relationship began;
- a country where a shared event happened;
- a future destination;
- a region connected to craft or material;
- a symbolic place that matters in the story.

The Source layer can then respond with relevant **categories, traditions, makers, materials, or DIY routes**.

## 4. Spatial routing examples

### Giver location supplied
The engine may emphasize:
- nearby makers;
- walkable sourcing;
- in-person experiences;
- hand delivery where appropriate.

### Recipient location supplied
The engine may emphasize:
- availability in the recipient's region;
- local cultural fit;
- delivery feasibility;
- time zone or postal practicality if needed.

### Symbolic origin supplied
The engine may emphasize:
- regionally meaningful materials;
- craft traditions;
- local publishing;
- food or scent provenance;
- place-linked objects;
- symbolic adaptation rather than literal purchase.

## 5. Provenance phrases

The Source branch may use language such as:
- "chosen from where this story began";
- "made near the place you still associate with that memory";
- "sourced to carry the geography of the moment";
- "adapt this locally if the original place is inaccessible."

Poetic phrasing must never imply factual provenance that has not been verified.

## 6. Data minimization

Spatial design must follow these rules:

- no precise location is required for core functionality;
- city/region-level input should be preferred when enough;
- no location history is created by default;
- no recipient address should be stored as relationship metadata;
- the system should not infer private locations;
- map/location APIs should receive the minimum data needed for the immediate task;
- exact addresses should only be processed when required for a user-requested sourcing or delivery action;
- any saved location must be explicitly user-controlled.

## 7. Safety and relational boundaries

Spatial symbolism can become intrusive if implemented carelessly.

The system must not encourage:
- surprise visits to homes or workplaces;
- tracking;
- repeated physical presence after rejection;
- leaving objects in prohibited/private spaces;
- "returning to where it began" when the place is unsafe or unwanted;
- location-based pressure in former relationships.

The poetic value of place does not override consent or safety.

## 8. Future memory mapping

Historical project plans imagined a future visual archive showing relational gestures across geography.

Any future mapping feature must be evaluated against the core doctrine:

> Does this map deepen memory, or turn relationships into a data collection?

A cumulative map should **not** become default telemetry.

A privacy-compatible future version could instead:
- render locally on-device;
- use user-selected coarse locations;
- store exported artifacts rather than server-side histories;
- remain entirely optional.

## 9. Technical contract

```yaml
spatial_input:
  giver_place:
    required: false
    precision: coarse_by_default
  recipient_place:
    required: false
    precision: coarse_by_default
  symbolic_origin:
    required: false
    precision: narrative

routing_effect:
  gift: low
  source: high
  ritual: medium

storage:
  default: ephemeral
```

## 10. Core principle

> Where a gift comes from can matter more than how efficiently it was found.

Spatial memory adds meaning only when it remains subordinate to the relationship and the user's own story.
