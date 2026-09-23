# 00 — Corpus & Exclusion Register

## A. Corpus lock

**Repository cut-off:** `f36bf74f984ba85149ef73345f8839dc9769379c`  
**Repository state at lock:** public; default branch `main`; branch protection reported `false`; no GitHub issues present at cut-off.

The locked tree contains **35 files**:

- 7 root governance/status files
- 14 canonical specification files under `docs/`
- 3 machine-readable registries under `data/`
- 11 files under `archive/source-extracts/` including its archive README

Audit files created after the cut-off are excluded from the object being audited.

## B. Direct primary project corpus

| ID | Artifact | Evidence class | Indexed extent / state |
|---|---|---|---|
| P-001 | Pius System Codex 5.0.pdf | DIRECT | 191 pages / 14,857 indexed lines |
| P-002 | Swedish Tech Sourcing Strategy for The Gift Whisperer.docx | DIRECT | 181 indexed lines |
| P-003 | Contributor Compliance & Collaboration Agreement.docx | DIRECT | 150 indexed lines |
| P-004 | The Gift Whisperer — THE RITUAL DECK.docx | DIRECT | 370 indexed lines |
| P-005 | The Gift Whisperer — THE STRATEGIC DECK.docx | DIRECT | 1,310 indexed lines |
| P-006 | The Gift Whisperer — Pitch Deck, Project plan, budget and workflow process.docx | DIRECT | 1,479 indexed lines |
| P-007 | Gift Whisperer Masterplan v.8.0.docx | DIRECT | 1,606 indexed lines |
| P-008 | The Gift Whisperer — Dev Brief — till Johan.docx | DIRECT | 148 indexed lines |
| P-009 | The-Gift-Whisperer.pptx | DIRECT text-accessible | 75 indexed text lines |
| P-010 | The-Gift-Whisperer-THE-STRATEGIC-DECK.pptx | DIRECT text-accessible | 432 indexed text lines |
| P-011 | Medarbetaravtal — Samarbets- och etiköverenskommelse.docx | DIRECT | 148 indexed lines |
| P-012 | GitHub repository `Hybrismannen/metoyo` at locked commit | DIRECT | 35 files |
| P-013 | Current METOYO consolidation + audit conversation | DIRECT | current chat only |

## C. External HARP verification corpus

Access date for all: **2026-09-23**.

| ID | Source | Use in audit |
|---|---|---|
| W-001 | ScienceDirect / Journal of Retailing: Otnes & McGrath (2001), DOI 10.1016/S0022-4359(00)00047-6 | verifies actual title/journal for mis-cited source |
| W-002 | Cele Otnes, University of Illinois publication profile | corroborates Otnes & McGrath bibliographic record |
| W-003 | SAGE / Political Theory: Wendy Brown (2006), DOI 10.1177/0090591706293016 | verifies actual Brown article title and journal details |
| W-004 | Google Books / Princeton records: Viviana Zelizer, The Social Meaning of Money | verifies 1994 edition metadata/publisher discrepancy |
| W-005 | University of Chicago Press: Maurice Godelier, The Enigma of the Gift | verifies source existence |
| W-006 | University of California Press: Hochschild, The Managed Heart | verifies source existence |
| W-007 | Google Books / catalog sources: Kimmel, Guyland | verifies source existence |
| W-008 | Notre Dame / Google Books: Klinenberg, Palaces for the People | verifies source existence |
| W-009 | David Graeber / University of Chicago distributed edition | verifies source existence |
| W-010 | Google Analytics / Google Tag Manager official documentation | verifies default GA4 data collection and cookie behavior |

## D. Summary-only evidence

| ID | Record | Status |
|---|---|---|
| S-001 | Prior METOYO Pius Lifetime Audit summary dated 2026-07-28 | SUMMARY-ONLY. The original audit report/chat is not retrievable in the current corpus. |
| S-002 | Prior statement that the July audit found 0 formal Atmos/ITR, Cellar, EPSc or HARP traces | SUMMARY-ONLY; not upgraded to direct evidence. |

Summary-only evidence can contextualize but cannot prove current compliance.

## E. Exclusion / missing-artifact register

| ID | Named or expected artifact | Audit treatment |
|---|---|---|
| X-001 | Original “PIUS LIFETIME AUDIT REPORT – [NAME] PROJECT LAB” directory/file | Not retrievable through current Files search. Protocol requirements were carried forward only where available from prior summary and Codex evidence. |
| X-002 | Full earlier METOYO development chats | Not retrievable as direct chat transcripts; not reconstructed. |
| X-003 | Masterplan v9.0 | MISSING. Strategic deck states “Masterplan v9.0 complete”; accessible supplied masterplan is v8.0. |
| X-004 | Standalone Persona Canon (20 entries) referenced in deck appendix | MISSING as standalone artifact. Persona content exists inside larger documents. |
| X-005 | Figma prototype/system deck | MISSING. Referenced in planning documents. |
| X-006 | Airtable persona-prompt-ritual matrix | MISSING. Referenced in architecture. |
| X-007 | Complete prompt-link library / “all prompt links ready” | MISSING. Dev brief says these existed/are ready, but they are not in the accessible source set. |
| X-008 | Live Carrd/Webflow implementation | MISSING / not in corpus. |
| X-009 | Signed contributor agreements | MISSING; only drafts/templates are present. |
| X-010 | Current grant applications / decisions | MISSING; historical funding plans only. |
| X-011 | Raw DOCX/PPTX binaries inside GitHub repository | MISSING from GitHub. Originals are available in the project environment but not preserved in the repository. |
| X-012 | HCC Seal of Accord / formal Pius clearance record for METOYO | NOT FOUND. |

## F. Archive-fidelity check

The GitHub archive claims to preserve text extracts from 10 supplied project artifacts.

Seven extracts are consistent in line-scale with their indexed originals after allowing for the archive header. Three are not:

| Source | Original indexed lines | GitHub extract lines | Audit result |
|---|---:|---:|---|
| Gift Whisperer Masterplan v.8.0 | 1,606 | 1,009 | **TRUNCATED** |
| Pitch Deck / Project plan / budget / workflow | 1,479 | 1,009 | **TRUNCATED** |
| Strategic Deck DOCX | 1,310 | 1,009 | **TRUNCATED** |

The Masterplan GitHub extract terminates during Spatial Memory Architecture rather than at the end of the source. The pitch extract terminates at the beginning of Go-to-Market. The strategic-deck DOCX extract terminates around the roadmap/visual suggestions.

Therefore the GitHub historical archive is **not source-complete at the audit cut-off**.
