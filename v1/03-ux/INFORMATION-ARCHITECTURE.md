# Information Architecture

## Public route tree

```
/
├── /begin
│   ├── relationship
│   ├── memory
│   ├── context
│   ├── result
│   └── refine
├── /about
├── /how-it-works
├── /privacy
├── /rituals
├── /accessibility
└── /reflection          optional entry

Authenticated/optional:
├── /save                gate only
└── /my-rituals          only if HD-004 enables persistence
```

## IA principle

The public experience should feel like one continuous ritual, not a dashboard. URL boundaries are implementation seams, not a reason to make the interface visually administrative.

## Navigation

Primary:
- METOYO mark/home
- Begin
- About

Secondary:
- How it works
- Privacy
- Accessibility

No persistent commerce/navigation clutter.

## Persona discovery

Until HD-001:
- all 20 relational roles remain available;
- constellation metadata must not be used for hidden filtering or model behavior;
- final grouping UI remains a swappable presentation layer.

## Progressive disclosure

The core experience asks only:
1. who the relationship is;
2. what the user remembers.

Tone, budget, time and spatial fields live under optional context.

## Exit architecture

Every ritual screen must provide a quiet exit/back route. The user should never feel trapped by sunk input.

## Responsive model

- Mobile: single-column ritual stack.
- Tablet: centered reading column with contextual side affordances.
- Desktop: max-width reading surface; optional contextual rail, never dashboard density.

## Accessibility

- semantic headings;
- keyboard-complete;
- no interaction depends on hover;
- no color-only meaning;
- reduced-motion mode;
- sufficient focus visibility;
- clear status announcements for generation/error;
- target WCAG 2.2 AA.
