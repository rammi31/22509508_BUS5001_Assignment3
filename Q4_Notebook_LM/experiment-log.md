# Q4 — NotebookLM Evaluation: Experiment Log

## Scenario

A postgraduate student preparing a briefing that compares how three major Melbourne-headquartered Australian companies, from different industries, approach ESG reporting.

## Sources loaded

Three published sustainability reports (PDFs held in `Company Reports/`):

1. ANZ — 2025 ESG Report (banking)
2. Telstra — 2024 Bigger Picture Sustainability Report (telecommunications)
3. BHP — 2024 sustainability reporting (mining)

## Tool

Google NotebookLM (free evaluation access). NotebookLM answers only from the loaded sources, not the open web. No code is involved; evidence is the queries, responses, and screenshots below.

---

## Experiments

### 1. Source-grounded summarisation

**Query:** "Summarise the main ESG priorities of each of the three companies in a few sentences each."

**Result:** Produced an accurate summary that kept each company's framework distinct: ANZ's seven material issues, Telstra's three pillars (doing business responsibly, creating a better digital world, sustaining our planet), and BHP's six-pillar social value framework. No blurring across sources.

**Finding:** Strong. Correctly synthesised three separate reports.

*Evidence: Screenshots/ (cross-source summary)*

---

### 2. Cross-document question answering

**Query:** "Compare how the three companies approach climate and carbon emissions. What targets has each set, and how do their approaches differ given their industries?"

**Result:** Generated a comparison table of operational (Scope 1 and 2), value-chain (Scope 3), and renewable-energy targets for all three companies, then explained each industry-specific approach with accurate detail (for example, ANZ's Large Emitters Engagement Program, Telstra dropping carbon offsets from FY25, BHP's reliance on partnerships for low-emission steelmaking).

**Finding:** Strong. Accurate, well-organised cross-document synthesis that would otherwise take hours of manual reading.

*Evidence: Screenshots/ (climate comparison)*

---

### 3. Inline citation accuracy

**Action:** Clicked the citation attached to the claim "100% renewable electricity at Chilean operations in CY2023".

**Result:** The citation opened the exact supporting passage in the BHP source document, confirming the claim traced to the correct report and a real passage.

**Finding:** Strong. Citations are verifiable and correctly attributed, which supports academic integrity.

*Evidence: Screenshots/ (expanded citation)*

---

### 4. Hallucination probe (reliability test)

**Query:** "What is each company's target for reducing single-use plastics in their offices, and what penalties do they impose on suppliers who fail to meet sustainability requirements?" (Information not present in the reports in this specific form.)

**Result:** NotebookLM stated plainly that none of the reports specify a standalone office single-use-plastics target, then offered the related information that genuinely is present (for example, ANZ's waste-to-landfill target, Telstra's packaging plastic reduction). It did not invent figures.

**Finding:** Strong. Because it answers only from sources, it resisted hallucination and was transparent about what was missing. This is the most important reliability result.

*Evidence: Screenshots/ (hallucination probe)*

---

### 5. Study material generation and Audio Overview

**Action:** Generated a briefing document and a podcast-style Audio Overview from the Studio panel. Outputs saved in `NotebookLM Output/`.

**Result:** Both generated successfully. The Audio Overview produced two AI voices discussing the material, with an interactive mode allowing questions to the narrators.

**Limitation found:** Both generated outputs defaulted to a single source (ANZ) rather than synthesising across all three loaded reports. When asked directly, the Audio Overview narrators confirmed they would only discuss ANZ. A user relying on the generated briefing without checking would receive a one-company view of a three-company task.

**Finding:** Mixed. The features are distinctive and useful, but the automated outputs were the least reliable part of the tool and need verification before use.

*Evidence: Screenshots/ (briefing and audio panel; ANZ-only limitation), NotebookLM Output/ (the generated artefacts)*

---

## Overall conclusion

NotebookLM is a strong aid for understanding and comparing sources, with verifiable citations and genuine resistance to hallucination. Its main weaknesses are that the automated generated outputs can be confidently incomplete (the single-source briefing and audio), and that it adds no critical perspective of its own, reporting source claims without questioning them. It is suitable for university adoption as a study and research aid, provided students verify its generated material and supply their own critical judgement.
