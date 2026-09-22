# 03 — Persona Canon

## 1. Persona logic

METOYO does not segment people by age, income, interests, purchase history or behavioral profile.

The Gift Whisperer uses **relational archetypes**. A persona represents the emotional field between giver and recipient, not the recipient's identity.

A persona supplies:
- prompt voice;
- emotional register;
- possible gesture grammar;
- symbolic vocabulary;
- likely intensity;
- common boundaries to respect.

## 2. Canon structure

The current canon contains **20 personas** across five constellations.

### A. Care & Tending

| Persona | Core relational function | Tone |
|---|---|---|
| The Mother | origin of care, nourishing presence | reverent · grounding · soft |
| The Father | structure, support, loyalty that may be under-spoken | quiet · grateful · strong |
| The Sibling | shared history, chaos, mirroring, survival | wry · tribal · honest |
| The Caregiver | one who showed up in need | subtle · humble · witnessing |
| The Self | inner companion; gifting as self-recognition | gentle · forgiving · empowering |

### B. Circumstantial

| Persona | Core relational function | Tone |
|---|---|---|
| The Neighbor | proximity, background allyship, everyday care | warm · observational · quiet |
| The Stranger Who Helped | brief but meaningful intervention | delicate · grateful · hushed |
| The Colleague | shared labor and daily rhythm | respectful · neutral · light |
| The Boss | authority relation with calibrated recognition | earnest · boundary-aware · cool |
| The Group | collective rhythm and shared identity | celebratory · communal · lively |

### C. Intimacy & Emotion

| Persona | Core relational function | Tone |
|---|---|---|
| The Romantic Other | longing, intimacy, chosen vulnerability | tender · magnetic · risk-aware |
| The Ex | relationship transformed by separation | bittersweet · grateful · mature |
| The Friend | chosen witness to a life | loyal · joyful · complex |
| The Child | care, wonder, growth and inherited future | proud · soft · receptive |
| The Muse | catalyst for art, imagination or longing | wordless · charged · surreal |

### D. Transformational

| Persona | Core relational function | Tone |
|---|---|---|
| The Mentor | guidance that enabled growth | grateful · reflective · anchored |
| The Lifechanger | person associated with a decisive shift | sacred · electric · precise |
| The Hero | model of courage, capacity or possibility | reverent · expansive · inspired |

### E. Philosophical

| Persona | Core relational function | Tone |
|---|---|---|
| The Future You | self as future relational other | speculative · soft · sincere |
| The Unknown | projected kindness without established relation | curious · open · symbolic |

## 3. Launch subset

Historical planning identified a smaller launch subset:

- The Romantic Other
- The Mentor
- The Friend
- The Lifechanger
- The Stranger Who Helped
- The Child
- The Ex

Optional early additions:
- The Sibling
- The Self
- The Neighbor

This is a historical MVP prioritization, not a statement that the remaining personas are deprecated.

## 4. Persona metadata

Each persona should be represented with:

```yaml
id:
name:
constellation:
core_function:
tone_palette:
prompt_set:
gesture_grammar:
gift_modalities:
boundary_notes:
icon:
color_field:
version:
status:
```

### Required distinction

- **Icon** is symbolic, not a literal portrait.
- **Color field** is an emotional signal, not demographic branding.
- **Prompt set** should contain multiple ways into the relational field.
- **Boundary notes** are mandatory for higher-intensity personas.

## 5. Prompt design

Prompts should evoke, not interrogate.

Useful prompt forms include:

### Associative memory
> What image comes to mind when you think of them at ease?

### Unnamed care
> What did they give you without knowing?

### Story flash
> Recall one thing they once said with pride. Where were you?

### Residual phrase
> What sentence of theirs still appears in your life?

### Unfinished gesture
> What deserves a second arrival?

The prompt should remain answerable with fragments. It should not force disclosure.

## 6. Persona does not equal diagnosis

A persona must never become:
- a psychological type;
- a personality score;
- a risk classification;
- a prediction of what the recipient wants;
- an excuse for manipulative advice.

"The Father" does not mean all fathers share one emotional grammar. It means the user has chosen to approach the memory through a father-relation lens.

## 7. Cultural adaptability

Persona meanings are culturally contingent.

Localization must therefore test:
- family-role assumptions;
- hierarchy;
- gift taboos;
- mourning and remembrance customs;
- intimacy norms;
- naming;
- symbolism;
- age and authority;
- anonymity and surprise.

A translated label is not sufficient localization.

## 8. Persona + gesture linkage

Each persona can map to several gesture grammars, but no gesture mode is mandatory.

Examples from the existing design:

- The Father → Silent Exchange / Hidden Offering
- The Mentor → Returned Place / Silent Exchange
- The Friend → Narrative Puzzle / Shared Ritual
- The Romantic Other → Returned Place / Narrative Puzzle / Shared Ritual
- The Stranger Who Helped → Hidden Offering
- The Self → Ritual Act / Hidden Offering
- The Child → Narrative Puzzle / Shared Ritual
- The Ex → Hidden Offering, with strong boundary calibration

## 9. Governance

Adding or changing a persona requires:
1. clear relational function;
2. evidence that it is not redundant with an existing persona;
3. tone and boundary definition;
4. prompt examples;
5. gesture mappings;
6. cultural-risk review;
7. versioning in the machine-readable registry.

The canon may evolve, but it should not expand simply to increase content volume.
