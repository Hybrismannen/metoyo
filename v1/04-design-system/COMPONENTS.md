# Component System

## Philosophy

Components should feel like instruments of attention, not app chrome.

## Core components

### RitualShell
Owns:
- max width;
- vertical rhythm;
- progress semantics;
- exit/back affordance;
- announcement region.

Does not own domain logic.

### MemoryFragmentInput
States:
- empty;
- active;
- filled;
- editing;
- error.

Rules:
- one short fragment per token;
- keyboard-first;
- removable;
- reorderable;
- no silent persistence.

### PersonaCard
Displays:
- persona label;
- one-sentence relational cue;
- optional icon.

Must not:
- show demographic assumptions;
- expose unresolved constellation as if settled.

### OptionalContextDisclosure
Collapsed by default.
Supports:
- budget;
- tone;
- time;
- DIY;
- place fields.

### TridentComposition
One semantic component with three arms:
- GiftPanel
- SourcePanel
- RitualPanel

All three must resolve before success state.

### MemoryLink
Explains why an output connects to submitted fragments.
Must use cautious language such as:
- “This draws on…”
- “This echoes…”

Never:
- “They are the kind of person who…”
- “You subconsciously…”

### RefinementSheet
Preset controls plus optional text.
Refinements change the proposal, not the persona identity.

### PrivacyCue
Compact inline disclosure that can open the full privacy explanation.
Must reflect real deployment behavior.

### SaveGate
Explains persistence before auth/storage.

### ReflectionJournal
Long-form optional text with no rating widgets.

### StatusMessage
Accessible live-region for:
- generating;
- retrying;
- validation errors;
- source failures.

## Interaction primitives

Buttons:
- Primary: one per screen maximum.
- Secondary: quiet outline/text.
- Destructive: explicit and rare.

Cards:
- content-led;
- no gratuitous hover lift;
- keyboard focus equivalent to pointer state.

Inputs:
- labels always visible;
- placeholder never substitutes for label;
- errors explain correction.

## Loading

Use:
- subtle line/ink animation;
- skeleton only for known layout.

Do not use:
- fake percentage;
- spinning dashboard indicators;
- gamified waiting copy.

## Empty states

Empty states should remain dignified:
- “Nothing has to be saved.”
- “You can leave this blank.”
- “There is no useful result yet.”

Never fill silence with unrelated recommendations.
