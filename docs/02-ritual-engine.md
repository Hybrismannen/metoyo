# 02 — The Gift Whisperer Ritual Engine & Trident

## 1. Role of the engine

The Gift Whisperer is the internal execution layer inside METOYO.

Its job is to convert a small amount of user-supplied relational memory into a structured set of possibilities without converting the relationship into a data profile.

## 2. Engine inputs

Primary:
- memory cluster;
- relational persona.

Optional:
- giver location;
- recipient location;
- symbolic origin;
- tone or mood;
- constraints such as budget, time, accessibility, handmade preference, distance, or delivery format.

These optional constraints must remain subordinate to the memory and relationship logic.

## 3. The Trident

The Trident is the stable output grammar:

```text
                 MEMORY
                   │
                   ▼
             RELATIONAL FIELD
                   │
                   ▼
           ┌───────┼────────┐
           │       │        │
         GIFT    SOURCE   RITUAL
           │       │        │
           └───────┼────────┘
                   ▼
               GESTURE
```

### 3.1 Gift

The **Gift** branch proposes what could carry the memory.

It may be:
- an object;
- a handmade artifact;
- a written message;
- an experience;
- an act;
- a shared activity;
- a symbolic intervention;
- a gesture-only gift.

A good Gift output should be:
- memory-aligned;
- symbolically intelligible;
- proportionate to the relationship;
- feasible or adaptable;
- non-generic;
- non-coercive.

If no object can carry the meaning well, the system should be willing to return an act, letter, conversation, or simple acknowledgment instead.

### 3.2 Source

The **Source** branch materializes the possibility.

It may include:
- local maker or shop category;
- DIY route;
- craft method;
- regionally meaningful object type;
- online source class;
- experience venue type;
- instructions for adapting an existing object;
- timing/logistical advice.

The source should not dominate the ritual. METOYO is not a shopping engine.

Preferred source hierarchy:
1. meaningful or local source;
2. maker / craft / slow route;
3. DIY or adapted route;
4. accessible conventional purchase if appropriate.

### 3.3 Ritual

The **Ritual** branch proposes how the gift could enter the relationship.

It includes:
- delivery mode;
- setting;
- timing;
- degree of speech or silence;
- optional wording;
- level of surprise;
- whether the gesture is private, shared, discovered, returned to place, or enacted together.

The ritual must always be presented as an invitation, not a command.

## 4. Gesture grammar linkage

The Ritual branch draws from six canonical gesture modes:

1. Hidden Offering
2. Returned Place
3. Silent Exchange
4. Narrative Puzzle
5. Ritual Act
6. Shared Ritual

See [Gesture Grammar](04-gesture-grammar.md).

## 5. Emotional sequencing

The Trident is more than a display format. It encodes a movement:

```text
internal evocation
      ↓
symbolic form
      ↓
material access
      ↓
embodied arrival
```

or, more simply:

```text
Memory → Matter → Encounter
```

## 6. Tone gates

The engine should control for tone such as:
- sincere;
- playful;
- reverent;
- restrained;
- tender;
- grateful;
- bold;
- delayed;
- bittersweet;
- celebratory.

Tone is not decoration. It calibrates the intensity of the suggestion.

A Father prompt, an Ex prompt, and a Child prompt should not generate identical emotional registers even when the memory cluster is similar.

## 7. Output quality tests

A Trident should be rejected or regenerated if:

- the Gift could fit almost anyone;
- the Source is simply a list of retailers;
- the Ritual is melodramatic relative to the relationship;
- the output invents facts about the recipient;
- the ritual crosses boundaries;
- the result is dependent on surveillance or stored profiling;
- the output commercializes grief, apology, trauma or reconciliation;
- the system speaks with unwarranted psychological certainty;
- the suggested geography is intrusive;
- the user would need to perform emotion rather than express it.

## 8. Example

### Input

```yaml
memory_cluster:
  - chalk
  - spiral
  - thesis
  - 2AM
  - margin
persona: The Mentor
tone: grateful
```

### Possible Trident

**Gift**  
A hand-bound notebook carrying selected marginal phrases from the work you completed together.

**Source**  
A local bookbinder or a simple hand-binding route using printed pages and linen thread.

**Ritual**  
Give it at the final meeting with very little explanation. Let the title and the collected marginalia carry the message.

This example is not a template to reproduce verbatim. It demonstrates the relationship between memory, symbolic object, feasible access, and delivery grammar.

## 9. Reflection seal

A Trident may end with an optional invitation:

> Would you like to return to this gesture later?

If accepted, the user enters the Reflection Chamber after an appropriate delay or at a time chosen by the user.

The reflection loop must not be designed to maximize return visits.

## 10. Room-violation test

Before release, any new Trident feature should be tested against the METOYO condition:

- Does this create room, or consume it?
- Does it invite, or interrupt?
- Does it support judgment, or replace it?
- Does it deepen presence, or increase dependence?
- Does it leave the relationship with the people involved, or pull it back into the system?

A feature that systematically fails this test should not ship.
