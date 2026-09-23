# METOYO Design Tokens — Candidate 1.0

**Status:** PROPOSED DEFAULT under HD-012.

The visual system translates the historical direction — parchment, misted glass, warm neutrals, light literary tactility, restrained Scandinavian/Japanese stationery references — into implementation tokens.

## Color

```css
:root {
  --paper-0: #FBF9F5;
  --paper-1: #F4F0E8;
  --ink-900: #25231F;
  --ink-700: #504B43;
  --ink-500: #7A746A;
  --line-200: #DDD6CA;

  --sage-100: #E7EBE2;
  --sage-500: #77816E;

  --clay-100: #F0E2D8;
  --clay-500: #A96F55;

  --mist-100: #E9ECEB;
  --mist-500: #748181;

  --focus: #2E5BFF;
  --danger: #8C2F2F;
}
```

Color is atmospheric, never demographic or persona-essential.

## Typography

Preferred roles:
- Display/ritual: high-quality editorial serif.
- Interface/body: humanist sans.
- System/metadata: same sans, smaller and quieter.

Implementation must use legally distributable fonts. No commercial font file is committed without license.

Suggested CSS stack until final font decision:

```css
--font-display: "Iowan Old Style", "Palatino Linotype", Georgia, serif;
--font-ui: Inter, ui-sans-serif, system-ui, sans-serif;
```

## Type scale

- display-xl: clamp(3rem, 7vw, 6.5rem)
- display-lg: clamp(2.25rem, 5vw, 4.5rem)
- h1: 2.25rem
- h2: 1.625rem
- h3: 1.25rem
- body-lg: 1.125rem / 1.7
- body: 1rem / 1.65
- small: .875rem / 1.5

## Spacing

4px base with generous macro-space:
- 1: 4
- 2: 8
- 3: 12
- 4: 16
- 6: 24
- 8: 32
- 12: 48
- 16: 64
- 24: 96
- 32: 128

## Radius

- chip: 999px
- card: 24px
- sheet: 32px
- input: 16px

## Shadow

Use soft ambient shadows only:
```
0 18px 60px rgba(40, 35, 28, 0.08)
```

## Motion

- default: 180–320ms
- page/ritual transition: 500–800ms
- no bounce;
- no confetti;
- no pulsing CTA;
- reduced motion removes spatial animation.

## Layout

Reading column: 680–760px.  
Ritual composition maximum: 1120px.  
Desktop whitespace is intentional; do not fill it with utility panels.
