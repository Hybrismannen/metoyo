# 01 — System Model & User Flow

## 1. System thesis

METOYO is a soft system for moving from **relational memory** to **meaningful gesture**.

The Gift Whisperer engine performs that transformation through a structured but non-deterministic sequence. The user retains interpretive control throughout.

## 2. Canonical flow

```text
1. Entry / pause
        ↓
2. Memory cluster
        ↓
3. Optional spatial memory
        ↓
4. Relational persona
        ↓
5. Curated prompt activation
        ↓
6. Trident generation
   Gift / Source / Ritual
        ↓
7. User judgment and adaptation
        ↓
8. Gesture in the world
        ↓
9. Optional Reflection Chamber
```

## 3. Entry condition

The system should not begin with a catalogue, search field, or shopping category. It should create a small threshold between urgency and action.

Typical entry language:
- "What do you remember?"
- "Is there someone you remember when you pause?"
- "Give 3–5 words. Not to explain. To evoke."

The interaction should feel like entering a quiet room rather than opening a store.

## 4. Memory cluster

The memory cluster is a short set of associative cues, typically **3–5 words or fragments**.

Examples:
- `rain / mint tea / silence / eyes`
- `wire / cocoa / midnight / glue`
- `chalk / spiral / thesis / margin`
- `apricot / jazz / train / warmth`

The cluster is not a profile. It is a temporary evocation device.

Its role is to activate:
- sensory memory;
- shared moments;
- unfinished meaning;
- relational tone;
- symbolic material;
- possible geography.

## 5. Optional spatial input

After memory entry, the user may optionally provide:
- where the giver is;
- where the recipient is;
- where the gift should feel as if it came from.

Spatial input is not required for core use. It exists to add symbolic or practical provenance to the **Source** branch of the Trident.

See [Spatial Memory Architecture](05-spatial-memory.md).

## 6. Relational persona

The user selects a relational archetype rather than a demographic segment.

A persona does not claim to define the recipient. It identifies a **relationship field** from which the prompt can speak.

Examples:
- The Mentor
- The Friend
- The Father
- The Romantic Other
- The Stranger Who Helped
- The Lifechanger
- The Ex
- The Self

The persona contributes:
- tone;
- likely emotional register;
- prompt grammar;
- compatible gesture modes;
- typical gift modalities.

See [Persona Canon](03-persona-canon.md).

## 7. Prompt activation

The engine combines:
- memory cluster;
- persona;
- optional spatial context;
- optional tone/mood filter;
- system ethical constraints;
- curated poetic grammar.

The system should not simply pass raw user input to a model and accept unfiltered output as authoritative.

Prompt architecture should instead:
1. preserve the user's own memory as primary evidence;
2. use the persona as relational context;
3. generate possibilities rather than conclusions;
4. avoid pretending to infer the recipient's inner state;
5. produce the Trident in a stable structure;
6. respect ethical and data-minimal constraints.

## 8. Trident output

Every complete interaction returns:

1. **Gift** — symbolic object, act, experience, message, or gesture.
2. **Source** — where/how to find it, make it, adapt it, or localize it.
3. **Ritual** — how the gesture could arrive.

The Trident is not three product recommendations. It is a choreography from memory to action.

See [Ritual Engine & Trident](02-ritual-engine.md).

## 9. User judgment gate

No Trident should bypass human judgment.

Before acting, the user should implicitly or explicitly test:
- Does this actually fit the person?
- Does it respect boundaries?
- Is the gesture culturally appropriate?
- Is the suggested ritual too intense?
- Would a simpler action be better?
- Is there any risk that surprise, anonymity, location, intimacy, or symbolism could become intrusive?

The system should make adaptation normal.

## 10. The real-world gesture

The system's purpose is fulfilled outside the interface.

Possible outputs include:
- a bought object;
- a handmade object;
- a letter;
- a shared meal;
- a returned place;
- a small ritual;
- an act of service;
- a message;
- a deliberate silence;
- an experience;
- a combination of these.

The object is not privileged over the act.

## 11. Reflection Chamber

After the gesture, the user may optionally return for reflective integration.

The Reflection Chamber is not a satisfaction survey. It exists to help the giver notice what happened and what they learned about giving.

See [Reflection Chamber](06-reflection-chamber.md).

## 12. Success condition

The system succeeds when it helps the user become more capable of:
- noticing;
- remembering;
- interpreting;
- giving;
- adapting;
- reflecting.

Repeat use is not automatically a positive KPI. Declining dependence can be evidence that the system worked.

## 13. Anti-patterns

A build is out of alignment if it:
- starts from products rather than memory;
- ranks people or relationships;
- profiles recipients;
- accumulates persistent relationship histories by default;
- turns the Trident into affiliate commerce;
- adds streaks, urgency, social comparison, points or reward loops;
- treats reflection as behavioral data extraction;
- makes the user feel that the system "knows" the recipient.

## 14. Minimal functional contract

A minimal METOYO implementation needs only:

```yaml
input:
  memory_cluster: required
  persona: required
  giver_location: optional
  recipient_location: optional
  symbolic_origin: optional
  tone: optional

output:
  gift: required
  source: required
  ritual: required
  reflection_invite: optional
```

Everything else is implementation detail unless explicitly promoted to canonical status.
