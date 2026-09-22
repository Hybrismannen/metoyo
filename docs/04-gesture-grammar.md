# 04 — Gesture Grammar

## 1. Purpose

In METOYO, the gift is not complete when an object is selected. Meaning is also carried by **how the gesture arrives**.

Gesture Grammar is the internal vocabulary used by The Gift Whisperer to compose the Ritual branch of the Trident.

The grammar is not a set of commands. It is a library of possible forms.

## 2. Canonical modes

There are six canonical gesture grammars.

### 2.1 Hidden Offering

**Principle:** the gift is discovered rather than formally delivered.

**Typical fit**
- The Self
- The Father
- The Stranger Who Helped
- The Ex, only when boundaries and safety clearly allow it

**Examples**
- left on a desk;
- placed beside a familiar object;
- slipped into a bag with consent-compatible context;
- mailed without ceremony;
- discovered during an ordinary routine.

**Emotional register**
- gratitude;
- closure;
- quiet care;
- reverence;
- restraint.

**Boundary rule**  
"Anonymous" or "surprise" must never be interpreted as permission for stalking, unwanted access, trespass, concealment that could frighten someone, or circumvention of a person's boundaries.

---

### 2.2 Returned Place

**Principle:** the gesture is connected to a place where the relationship or memory carries meaning.

**Typical fit**
- The Romantic Other
- The Mentor
- The Lifechanger
- The Friend

**Examples**
- given during a walk near an old campus;
- sourced from the place where a shared memory began;
- presented during a return visit;
- accompanied by a map, image, or reference to place.

**Emotional register**
- intimacy;
- narrative return;
- gratitude;
- continuity;
- renewal.

**Boundary rule**  
The system should not encourage uninvited appearances at private homes, workplaces, schools, memorial spaces, or other sensitive locations.

---

### 2.3 Silent Exchange

**Principle:** the object or act carries most of the message.

**Typical fit**
- parent figures;
- The Colleague;
- The Boss;
- The Mentor;
- relationships where overt sentiment could feel disproportionate.

**Examples**
- handed over after a meeting with a simple acknowledgment;
- set on a table;
- given with a short "thank you";
- paired with one restrained line rather than a speech.

**Emotional register**
- respect;
- maturity;
- acknowledgment;
- dignity.

---

### 2.4 Narrative Puzzle

**Principle:** the gift arrives through clues, sequence, or layered discovery.

**Typical fit**
- The Friend
- The Child
- The Group
- The Romantic Other

**Examples**
- treasure map;
- clues tied to shared memories;
- nested notes;
- a poem that points toward the gift;
- staged discovery across several small artifacts.

**Emotional register**
- play;
- anticipation;
- co-creation;
- surprise.

**Boundary rule**  
Puzzles should remain optional and enjoyable. Do not make emotional access contingent on solving something difficult, humiliating, public, or socially risky.

---

### 2.5 Ritual Act

**Principle:** the gift is embedded in a self-designed micro-ritual.

**Typical fit**
- The Future You
- The Self
- The Muse
- symbolic life transitions

**Examples**
- writing and sealing a future letter;
- lighting a candle before opening a text;
- creating a private sequence of music, reflection and object;
- placing an artifact in a chosen personal space.

**Emotional register**
- anchoring;
- transformation;
- reflection;
- intentionality.

**Boundary rule**  
Ritual language must not imply supernatural efficacy, therapeutic cure, or moral obligation.

---

### 2.6 Shared Ritual

**Principle:** giver and recipient enact the gift together.

**Typical fit**
- The Child
- The Friend
- The Romantic Other
- The Group

**Examples**
- cook the meal together;
- brew and taste something together;
- read or listen together;
- make or finish the object together;
- visit a meaningful place together.

**Emotional register**
- presence;
- trust;
- joy;
- co-creation.

## 3. Mode selection

The engine can propose a gesture mode based on:
- persona;
- memory cluster;
- tone;
- geography;
- practical constraints;
- relational intensity.

But the final mode remains the user's choice.

## 4. Ritual output structure

A Ritual output may contain:

```yaml
mode:
tone:
setting:
timing:
delivery:
optional_words:
adaptation_note:
boundary_note:
```

The `boundary_note` is especially important for:
- surprise;
- anonymity;
- romantic contexts;
- former partners;
- children;
- workplace hierarchy;
- geographic return;
- grief;
- apology;
- reconciliation.

## 5. Design standard

A good ritual:
- makes the memory more legible;
- does not overpower the recipient;
- is proportionate to the relationship;
- can be simplified;
- does not require public performance;
- preserves the recipient's freedom to respond or not respond.

## 6. Anti-patterns

Reject ritual suggestions that:
- manufacture pressure;
- stage emotional ambushes;
- require trespass or covert access;
- exploit children or subordinates;
- use public embarrassment;
- demand forgiveness;
- romanticize obsessive persistence;
- infer consent from past intimacy;
- treat grief or trauma as theatrical material.

## 7. Core formulation

> The presentation is part of the gift, but the recipient is never part of the staging.

The ritual should carry care into the encounter without scripting the other person's reaction.
