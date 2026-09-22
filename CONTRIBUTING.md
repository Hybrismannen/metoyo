# Contributing to METOYO

## Read first

Before proposing a change, read:

1. [Canonical identity](docs/00-canonical-identity.md)
2. [System model](docs/01-system-model.md)
3. [Ethics, privacy and governance](docs/07-ethics-privacy-governance.md)
4. [History and provenance](HISTORY.md)
5. [Source index](SOURCE_INDEX.md)

## Contribution principle

METOYO should not accumulate features simply because they are technically possible.

A useful contribution must strengthen at least one of:
- ritual clarity;
- relational fit;
- human agency;
- privacy;
- accessibility;
- cultural adaptability;
- technical reliability;
- provenance;
- evaluation quality.

## Required change note

Any substantive PR should state:

```markdown
### Purpose
What problem does this solve?

### Canonical impact
Which METOYO rule or module does it affect?

### Data impact
Does it add collection, persistence, inference, logging or third parties?

### Ritual impact
Does it alter the user flow, Trident, personas, gesture grammar or reflection?

### Boundary check
Could it increase pressure, intrusion, manipulation or emotional overreach?

### Provenance
What source or decision supports the change?

### Reversibility
Can the user decline or undo the new behavior?
```

## Historical files

Do not normalize historical wording just for consistency.

In particular, do not blindly replace **The Gift Whisperer** with **METOYO**.

The public/internal distinction is architectural:
- METOYO = public ritual space;
- The Gift Whisperer = internal engine.

## New personas

A new persona must include:
- distinct relational function;
- constellation;
- tone;
- prompt logic;
- gesture modes;
- boundary notes;
- localization considerations.

## New gesture modes

A new gesture mode must:
- be genuinely distinct from the six canonical modes;
- describe a form of arrival, not a product category;
- include safety/boundary analysis;
- remain optional.

## New analytics

Treat analytics as a high-scrutiny change.

A PR adding analytics must explain why aggregate service quality cannot be measured with less data.

No hidden relational profiles, emotional scoring, advertising audiences, or retention optimization.

## New model/provider

Document:
- data retention;
- training use;
- region/data residency where relevant;
- structured output capability;
- privacy controls;
- failure modes;
- cost;
- replacement plan.

The model provider is replaceable infrastructure, not project identity.

## Research and factual claims

Use the evidence types in [SOURCE_INDEX.md](SOURCE_INDEX.md).

Do not convert a project hypothesis into a factual claim without independent evidence.

## Tone

Public copy should be:
- restrained;
- clear;
- lightly poetic where useful;
- non-performative;
- non-coercive.

Avoid startup hype, exaggerated impact claims, and language that makes the system appear to know users or recipients better than they know themselves.

## Licensing

By contributing project material, contributors should ensure they have the right to do so and understand the repository's CC BY-NC-SA 4.0 posture, subject to any file-specific notice.
