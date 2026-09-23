# Gift Whisperer Orchestration

## Role

The Gift Whisperer is the internal orchestration engine. It is not presented as an autonomous relational authority.

## Pipeline

```
Client request
→ normalize
→ validate
→ persona policy
→ boundary/safety policy
→ prompt assembly
→ model adapter
→ structured-output validation
→ source adapter (optional)
→ ritual validator
→ response normalizer
→ client
```

## Inputs

Only the fields declared in `trident-contract.yaml`.

No hidden enrichment from:
- contacts;
- browsing history;
- advertising profiles;
- recipient social accounts;
- inferred protected traits.

## Prompt assembly layers

1. system identity and product invariant;
2. Trident schema;
3. persona relational logic;
4. memory fragments;
5. optional context;
6. safety/boundary instructions;
7. refinement instruction;
8. output schema.

The raw user input is not allowed to override higher-order product/safety instructions.

## Model adapter

Interface:

```ts
interface RitualModel {
  generate(input: NormalizedRitualRequest): Promise<StructuredTridentDraft>
}
```

Provider-specific implementation stays behind the interface.

## Source adapter

Source enrichment is optional and downstream of meaning generation.

The model should first determine what kind of thing/action fits. Source routing then answers how it might be obtained or made.

This prevents product availability from deciding meaning.

## Validation

A draft is rejected when:
- any Trident arm is absent;
- output invents recipient facts;
- source is an ad/affiliate ranking presented as neutral;
- ritual creates coercion or unsafe surprise;
- rationale makes psychological claims;
- content violates persona boundary rules.

One repair pass is allowed. If still invalid, return a recoverable failure state rather than fabricated output.

## Human judgment gate

The engine output is never an instruction to act. UI language must support alteration/rejection.

## Logging

Provider/server logs must contain only what is necessary for operations and must conform to the data lifecycle contract.
