# Test Plan

## Layers

### 1. Unit
- schema validation;
- state transitions;
- refinement mapping;
- event allowlist;
- privacy serialization;
- source adapter degradation.

### 2. Component
- memory fragment keyboard interactions;
- persona selection;
- disclosure panels;
- Trident composition;
- error states;
- Save Gate.

### 3. Contract
- API request/response;
- model adapter;
- persistence adapter;
- telemetry adapter.

### 4. Prompt regression
Maintain fixture set across:
- personas;
- tones;
- low-information memory;
- conflicting memory;
- low/no budget;
- no-object refinement;
- unsafe requests.

Each fixture evaluates:
- schema;
- memory specificity;
- safety;
- non-genericity;
- unsupported inference.

### 5. Security
- RLS allow/deny;
- auth boundaries;
- secret scanning;
- prompt injection against memory/refinement fields;
- stored XSS where persistence exists;
- API rate limiting.

### 6. Privacy
- guest path network trace;
- storage inspection;
- cookie inspection;
- server-log sampling;
- delete/export verification.

### 7. Accessibility
Automated + manual:
- keyboard;
- screen reader;
- zoom;
- reduced motion;
- contrast;
- touch targets.

### 8. Visual regression
Reference:
- key mobile sizes;
- tablet;
- desktop;
- reduced motion.

### 9. Ritual QA
Human review asks:
- does this feel like one offering?
- is it too generic?
- does Source dominate?
- is the Ritual performative/pressuring?
- does rationale overclaim?

## Release gate

A failing critical privacy, authorization, safety or Trident-contract test blocks release.
