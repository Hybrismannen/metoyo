# 05 — Correction / Failure / Contradiction Register

Severity scale:
- **CRITICAL** — blocks baseline lock / breaks provenance or human authority.
- **HIGH** — material system contradiction or evidence failure.
- **MEDIUM** — significant control, implementation or clarity debt.
- **LOW** — localized weakness not independently blocking.

## Register

| ID | Severity | Finding | Evidence state | Audit disposition |
|---|---|---|---|---|
| F-001 | CRITICAL | Three GitHub source extracts are truncated at 1,009 total lines despite longer originals. | DIRECT | OPEN — baseline blocker |
| F-002 | CRITICAL | Assistant-created `DECISIONS.md` presents some derived/inferred choices as settled canonical human decisions without ratification trace. | DIRECT + Codex | OPEN — authority blocker |
| F-003 | HIGH | Raw DOCX/PPTX source binaries are absent from GitHub; visual/layout provenance is not repository-preserved. | DIRECT | OPEN |
| F-004 | HIGH | Masterplan v9.0 is referenced as complete but is not in accessible corpus; only v8.0 supplied. | DIRECT | OPEN |
| F-005 | HIGH | Persona constellation assignments conflict across Masterplan and Strategic Deck; current canon is a hybrid supported by neither source as a whole. | DIRECT | OPEN |
| F-006 | HIGH | “No tracking / no third-party analytics / no cookies” conflicts with GA4, Tag Manager, Bitly/UTM, Looker and engagement-event instrumentation. | DIRECT + EXTERNAL-VERIFIED | OPEN |
| F-007 | HIGH | HARP failure: Otnes/McGrath citation has wrong title and journal. | DIRECT + EXTERNAL-VERIFIED | OPEN |
| F-008 | HIGH | HARP failure: Wendy Brown 2006 citation title is wrong; actual article is “American Nightmare: Neoliberalism, Neoconservatism, and De-Democratization.” | DIRECT + EXTERNAL-VERIFIED | OPEN |
| F-009 | HIGH | Broughton 2022 “The Invisible Work of Holiday Gifting” in The Atlantic could not be verified in targeted search. | DIRECT + EXTERNAL SEARCH | OPEN / unverified |
| F-010 | MEDIUM | Zelizer 1994 citation lists Princeton University Press; accessible 1994 record identifies Basic Books. | DIRECT + EXTERNAL-VERIFIED | OPEN metadata error |
| F-011 | HIGH | Claim that men are statistically less likely to plan, personalize or emotionally reflect on gifting is not supported by the cited references as presented; the key Otnes item is a male-shopping paper, not the cited gift-giving study. | DIRECT + EXTERNAL-VERIFIED | OPEN |
| F-012 | HIGH | “Zero competitors / no tool today / first mover” claims lack a documented market-scan evidence trail in the accessible corpus. | DIRECT | OPEN as unverified historical claim |
| F-013 | MEDIUM | Literal public copy “stores nothing / tracks nothing / remembers no one” conflicts with optional save ritual/reflection/email/logging concepts. | DIRECT | OPEN semantic/implementation contradiction |
| F-014 | MEDIUM | Strategic claim “no raw user text is ever directly injected into model” sits in tension with the dev flow where user memory keywords are inserted into prestructured ChatGPT prompts. | DIRECT | OPEN |
| F-015 | MEDIUM | Contributor/legal documents are templates/drafts, not signed or legally cleared execution instruments; GDPR-compliant claims remain aspirational without deployment evidence. | DIRECT | OPEN |
| F-016 | MEDIUM | Future executable software license is unresolved; historic “all work CC BY-NC-SA” and current documentation-only license caveat are not yet a single ratified software policy. | DIRECT | OPEN |
| F-017 | MEDIUM | YAML registries are machine-readable but no CI/schema validation/test evidence exists. | DIRECT | OPEN |
| F-018 | MEDIUM | GitHub `main` is unprotected; inspected commits report unsigned verification; no issue register existed at cut-off. | DIRECT GitHub | OPEN control-state finding |
| F-019 | MEDIUM | Current decisions lack per-decision source pointer, authorizing human, date of ratification and supersession relation. | DIRECT | OPEN |
| F-020 | MEDIUM | Source extracts do not carry source hashes/checksums or extraction range metadata proving exact fidelity. | DIRECT | OPEN |
| F-021 | MEDIUM | Pius lineage is direct, but formal METOYO EPSc/Atmos/HARP/HCC pre-audit traces are not evidenced. | DIRECT / absence finding | OPEN |
| F-022 | MEDIUM | The current `PROJECT_STATUS.md` marks historical source extracts “Archived” without exposing that three are truncated; status presentation is materially incomplete. | DIRECT | OPEN |
| F-023 | MEDIUM | Previous assistant statement that the source preservation pass was complete was false at the locked state because three long extracts were incomplete. | DIRECT current chat + repo | CORRECTION LOGGED |
| F-024 | LOW | Historical roadmap, funding and technology labels are date-bound 2025 material and can be misread as current if archive context is skipped. | DIRECT | OPEN contextual risk |

## Correction event

### C-001 — “Everything is now preserved”

Prior assistant output stated that all 10 source artifacts had been preserved in GitHub as historical text extracts.

Audit finding:
- ten extract files exist;
- three are truncated;
- no raw binaries are in the repository.

**Correction:** existence of an extract file is not equivalent to complete preservation.

## Contradiction clusters

### Cluster A — Privacy
No tracking / no cookies / no third-party analytics  
**versus**  
GA4 / Tag Manager / Bitly / UTM / Looker / dwell & click metrics.

### Cluster B — Persona ontology
Masterplan taxonomy  
**versus**  
Strategic Deck taxonomy  
**versus**  
current hybrid canon.

### Cluster C — Architecture authority
Naming directive says system architecture remains unchanged  
**versus**  
current D-015 demotes old vendor stack to noncanonical infrastructure.

### Cluster D — Source authority
Strategic Deck says Masterplan v9.0 complete  
**versus**  
only v8.0 accessible.

### Cluster E — Privacy rhetoric vs persistence
“Stores nothing”  
**versus**  
save ritual / reflection / email reminder / technical logs.

### Cluster F — Human authority
Pius Ex-Inerta demands protocol/human tether  
**versus**  
assistant-generated unratified canonical decisions.

## No-Suggestion Firewall

This register records state and contradiction only. It does not prescribe redesign or remediation.
