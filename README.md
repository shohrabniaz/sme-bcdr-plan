# Business Continuity and Disaster Recovery Plan for a Professional Services SME

**Author:** Md Shohrab Hossen Niaz  
**Focus:** bcdr  
**Visibility guidance:** public-ok

## Overview

Matches HA/DR/cloud spend work you already do; research packaging for resilience.

## Research questions

1. What business problem does “Business Continuity and Disaster Recovery Plan for a Professional Services SME” solve for an SME or partner organisation?
2. Which artefacts demonstrate a credible, implementable solution?
3. How is success measured without overstating lab or synthetic evidence?

## Deliverables

- BIA summary
- BC/DR outline
- exercise schedule
- Report and presentation (`Final_Submission/`)
- Evaluation scorecard (`02_Evaluation/`)
- Design notes (`01_Design/`)
- Baseline evidence JSON (`evidence/`)

## Repository layout

```
01_Design/           Design and method notes
02_Evaluation/       Scorecard workbook
evidence/            Baseline evidence model
Final_Submission/    Report, slides, appendices
```

## Limits

Synthetic or laboratory baselines are labelled. No production tenant secrets. Where a topic could imply offensive techniques, this pack stays defensive and high-level.

**GitHub:** `sme-bcdr-plan`


## Run the automation

Working code is in `src/`. Sample inputs are in `data/`. Results write to `output/`.

```powershell
.\automation\run.ps1
```

Manual:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -r requirements.txt
python -m src.cli run
python tests\test_smoke.py
```

Domain engine kind: `bcdr`.

**Author:** Md Shohrab Hossen Niaz  
**GitHub:** `sme-bcdr-plan`
