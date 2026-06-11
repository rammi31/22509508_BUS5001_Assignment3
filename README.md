# BUS5001 Assignment 3 — Experiment Logs

Supporting experiment logs and evidence for Questions 3 and 4 of BUS5001 Assignment 3. The full written analysis is in the submitted report; this repository holds the runnable notebook, screenshots, and experiment records.

## Repository structure

```
.
├── Q3_LLM_Triage/
│   ├── 22509508_Assignment3_LLM_Triage.ipynb   # the triage system notebook
│   ├── requirements.txt
│   └── Screenshots and Outputs/                # key outputs
│
└── Q4_NotebookLM/
    ├── experiment-log.md                       # queries run and findings
    ├── Company Reports/                        # the three source PDFs
    ├── NotebookLM Output/                      # generated briefing and audio overview
    └── Screenshots/                            # evidence of each feature tested
```

## Q3 — ESG Operational Message Triage System

A prototype that uses a large language model (Claude Haiku, via the Anthropic API) to classify and triage ESG-related operational messages, then route each one to the right team or escalate it for human review. The notebook covers the improved prompt, single-run classification, a five-run consistency experiment, a Hugging Face zero-shot baseline comparison, and a triage system with schema validation, a safe fallback, and multi-issue splitting.

To run it: open the notebook in Google Colab, add your Anthropic API key as a Colab secret named `ANTHROPIC_API_KEY`, then run all cells. No API key is stored in the notebook.

## Q4 — Evaluation of NotebookLM

An evaluation of Google's NotebookLM as a cloud-based AI learning tool, using three Australian sustainability reports (ANZ, Telstra and BHP) as sources. The experiment log records the queries run, the tool's responses, and the findings, including a hallucination probe and an observed limitation in the generated outputs. NotebookLM is a hosted tool with no local code, so the evidence is the experiment log, the generated outputs, and the screenshots.

## Note on credentials

No API keys or credentials are stored anywhere in this repository.
