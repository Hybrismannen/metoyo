# 08 — Technical Architecture

## 1. Architectural principle

The technical stack must remain subordinate to the ritual architecture.

The original Gift Whisperer plans deliberately favored a light implementation because the system's value was expected to come from:
- prompt composition;
- relational logic;
- tone;
- ritual choreography;
- data restraint;

rather than heavy application infrastructure.

This file distinguishes **canonical requirements** from **historical implementation proposals**.

---

## 2. Canonical functional architecture

```text
┌───────────────────────────────────────────────┐
│                  METOYO UI                    │
│     public ritual space / narrative shell     │
└───────────────────┬───────────────────────────┘
                    │
                    ▼
┌───────────────────────────────────────────────┐
│          GIFT WHISPERER ORCHESTRATOR          │
│ memory + persona + optional context + policy  │
└───────┬───────────────────────┬───────────────┘
        │                       │
        ▼                       ▼
  Prompt assembly          Safety / tone gate
        │                       │
        └─────────────┬─────────┘
                      ▼
               Model execution
                      │
                      ▼
             Trident normalizer
          Gift / Source / Ritual
                      │
        ┌─────────────┴─────────────┐
        ▼                           ▼
 optional source lookup       optional reflection
 / spatial routing            invitation
```

## 3. Canonical components

### 3.1 Presentation layer

Must support:
- calm, mobile-capable interaction;
- low cognitive load;
- narrative pacing;
- persona selection;
- memory entry;
- optional spatial input;
- readable Trident output;
- easy exit.

No account should be required unless a feature genuinely requires persistence.

### 3.2 Ritual configuration layer

Stores non-user system content:
- personas;
- prompt templates;
- tone maps;
- gesture grammar;
- boundary rules;
- output schemas;
- localization variants;
- version metadata.

This is **system configuration**, not a relationship database.

### 3.3 Orchestration layer

Responsible for:
- receiving ephemeral user input;
- applying persona/tone/gesture context;
- building the model request;
- enforcing output schema;
- applying post-generation checks;
- discarding or returning ephemeral data according to policy.

### 3.4 Model provider layer

The model is replaceable.

No provider name is part of METOYO's core ontology.

Any model/provider must be evaluated for:
- retention;
- training use;
- data residency;
- privacy controls;
- latency;
- prompt fidelity;
- structured-output support;
- safety behavior;
- cost.

### 3.5 Source layer

If actual sourcing is enabled, it should be modular.

Possible source types:
- local business search;
- maker directories;
- web search;
- handcraft/DIY guidance;
- user-specified sources;
- place-aware lookup.

The Source layer must not silently become an affiliate engine.

### 3.6 Reflection layer

Optional and logically separable from core generation.

No reflection persistence is required for the base system.

---

## 4. Historical stack proposals

The 2025 materials proposed combinations including:

| Layer | Historical proposal |
|---|---|
| Frontend | Carrd or Webflow |
| Prompt engine | GPT-4; optional Claude |
| Persona/ritual database | Airtable |
| Input/forms | Typeform or Tally |
| Link tracking | Bitly / UTM |
| Analytics | GA4 / Tag Manager / Looker Studio |
| Automation | Zapier |
| Design system | Figma |
| Collaborative content | Notion, optional |

These are **historical design choices**, not canonical dependencies.

Some of them also conflict in tension with stronger later privacy principles if deployed conventionally. Any contemporary build should reassess them rather than copy them mechanically.

---

## 5. Recommended modern repository architecture

A future code implementation can remain provider-neutral:

```text
/apps
  /web

/packages
  /ritual-core
  /persona-registry
  /prompt-compiler
  /trident-schema
  /policy
  /source-adapters
  /localization

/content
  /personas
  /prompts
  /gesture-grammar
  /ritual-copy

/docs
/data
/tests
```

This repository currently prioritizes specification before implementation.

## 6. Data lifecycle

### Default interaction

```text
user input
   ↓
ephemeral request object
   ↓
prompt compiler
   ↓
model/provider
   ↓
normalized Trident
   ↓
display
   ↓
discard transient state
```

### Persistence should require a separate user action

Examples:
- save a ritual;
- export a result;
- save a reflection;
- schedule a reminder.

## 7. Schema discipline

Outputs should be structurally validated.

See [Trident schema](../data/trident-schema.yaml).

Recommended logical shape:

```json
{
  "gift": {},
  "source": {},
  "ritual": {},
  "reflection_invite": {}
}
```

Natural language remains important, but a stable schema makes it possible to:
- validate completeness;
- apply policy checks;
- render consistently;
- localize;
- test regressions;
- switch model providers.

## 8. Prompt separation

Maintain distinct layers:

1. **canonical policy**
2. **persona definition**
3. **gesture grammar**
4. **user memory**
5. **optional context**
6. **output contract**

Do not bury all logic in one unversioned prompt.

## 9. Analytics doctrine

Historical materials proposed light interaction analytics. Current implementation must distinguish:

### Acceptable operational metrics
- anonymous uptime/error rate;
- aggregate completion counts if privacy-preserving;
- performance/latency;
- opt-in research metrics.

### High-risk / misaligned metrics
- cross-session relationship histories;
- individual emotional funnels;
- recipient profiling;
- retention optimization;
- personalized behavioral nudging;
- user-level emotional scoring.

METOYO does not need an engagement surveillance stack to prove that it works.

## 10. Security

At minimum:
- no secrets in client code;
- environment-bound provider keys;
- strict logging hygiene;
- input length limits;
- model output validation;
- abuse and prompt-injection handling for any external lookup layer;
- dependency monitoring;
- privacy review for every third-party service.

## 11. Accessibility

The poetic interface must still be usable.

Requirements should include:
- semantic HTML;
- keyboard navigation;
- sufficient contrast;
- screen-reader support;
- reduced-motion behavior;
- plain-language alternatives where ritual copy becomes ambiguous;
- no essential meaning conveyed only by color/iconography.

## 12. Implementation test

A technical choice is good for METOYO only if it passes all four:

1. **Does it serve the ritual?**
2. **Does it minimize unnecessary data?**
3. **Can it be replaced without rewriting the ontology?**
4. **Does it preserve human interpretive agency?**

Technology is infrastructure. It is not the identity of the project.
