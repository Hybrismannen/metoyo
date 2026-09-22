# 12 — Editorial & Source Protocol

## 1. Purpose

METOYO uses poetic and symbolic language. That makes source discipline more important, not less.

This protocol adapts the Pius/HARP commitment to reference control into a practical repository standard.

## 2. Four evidence classes

Every consequential statement should be identifiable as one of:

### A. Project decision
A rule intentionally adopted by the project.

Examples:
- METOYO is the public identity.
- The Gift Whisperer is the internal engine.
- The Trident is Gift / Source / Ritual.
- Forget-by-default is a design principle.

### B. Project hypothesis
A proposition to test.

Examples:
- memory prompts may reduce gift anxiety;
- using the system may strengthen confidence in giving;
- disappearing-system design may support autonomy.

### C. Historical plan
A dated choice or proposal.

Examples:
- Carrd as frontend;
- Airtable as persona store;
- a 145,000 SEK pilot budget;
- a December 2025 public launch target.

### D. External claim
A factual statement about the world requiring independent verification.

Examples:
- behavioral or gender research;
- legal compliance;
- market size;
- competitor absence;
- current grant eligibility;
- current provider privacy practices.

## 3. Source hierarchy

Prefer:
1. primary project decision records for project decisions;
2. original source documents for historical provenance;
3. primary academic, legal, official or first-party sources for external claims;
4. strong secondary syntheses when primary material is unavailable.

Avoid using:
- unsourced deck placeholders;
- inherited claims repeated across project documents;
- marketing pages as sole evidence for independent impact;
- AI-generated citations that have not been checked.

## 4. Historical fidelity

Do not "correct" history by rewriting it.

If a source says:
- The Gift Whisperer;
- GPT-4;
- Carrd;
- Airtable;
- a 2025 date;

preserve it in the archive.

In canonical docs, explain whether the item is still binding.

## 5. Citation discipline

For public-facing research material:
- use Harvard-style references unless another format is explicitly chosen;
- include stable identifiers/URLs where possible;
- verify author, title, year and publisher;
- distinguish quotation from paraphrase;
- record access date for web sources when appropriate.

## 6. Claim audit

Before publication, scan for:

### Causal verbs
"improves", "reduces", "increases", "changes", "causes".

### Universal claims
"people", "men", "women", "everyone", "no tool".

### Market claims
"first", "only", "unique", "zero competitors".

### Legal claims
"GDPR-compliant", "anonymous", "fully private".

### Technical claims
"stores nothing", "trains on nothing", "no tracking".

These statements are high-risk because implementation or evidence may not support them literally.

## 7. Privacy language rule

Never publish a stronger privacy claim than the deployed architecture can prove.

For example:

**Preferred when true**
> Inputs are processed ephemerally by METOYO and are not stored by the METOYO application.

**Requires additional verification**
> No third party retains any input.

The second depends on provider contracts and configuration.

## 8. Narrative examples

Fictional/composite user stories can be useful, but they must not be presented as documented real testimonials.

Label as appropriate:
- fictional vignette;
- composite scenario;
- illustrative example;
- anonymized real case, only with appropriate consent.

## 9. Audit record

For a major publication or research deck, maintain:

```yaml
publication:
version:
date:
claims_reviewed:
sources_checked:
privacy_language_checked:
historical_vs_current_checked:
reviewer:
open_questions:
```

## 10. Repository enforcement

A substantive PR introducing external factual claims should identify its sources in the PR description.

If evidence is missing:
- mark the statement as hypothesis;
- remove the claim;
- or create a research task.

Do not silently fill gaps with plausible language.

## 11. Editorial rule

> Poetic precision and factual precision are separate obligations. METOYO requires both.
