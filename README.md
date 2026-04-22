# AI-Facial-Recognition
# AI Facial Recognition — Compliance Intelligence Explorer

> **7CS525 Human & Legal Aspects of Cyber Security**  
> University of Derby · MSc Cybersecurity 2025/26 · Student: 100796311

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YOUR-USERNAME/YOUR-REPO/blob/main/AI_Facial_Recognition_Compliance_Explorer.ipynb)

---

## Overview

This notebook maps the **compliance status of a deployed AI facial recognition access control system** against every applicable legal obligation — producing interactive visualisations that support legal argument, risk governance and board-level reporting.

The system analysed is a UK retail bank deploying biometric building access control across three sites (~4,500 employees). It is classified as **HIGH RISK** under EU AI Act Annex III Point 1 and simultaneously engages the **Article 5(1)(h) prohibition** — making it the most heavily regulated AI category in Europe.

---

## What Makes This Notebook Different

Unlike generic EU AI Act reference tools, this notebook maps **compliance status of a specific deployed system** against each legal obligation — including cross-regime alignment with UK GDPR, Equality Act 2010, RRO 2005, FCA Consumer Duty, and the Bridges v SWP [2020] precedent.

---

## Modules

| # | Module | Output |
|---|--------|--------|
| 1 | **System Architecture Pipeline** | Interactive processing flow with stakeholder touchpoints |
| 2 | **EU AI Act Dual-Regime Analysis** | Art.5(1)(h) prohibition + Annex III high-risk tier cards |
| 3 | **Articles 9–15 Applied** | 7 compliance cards with GAP/PARTIAL/MET status and legal references |
| 4 | **EU vs UK Regulatory Comparison** | Side-by-side 6-row comparison table |
| 5 | **Accountability Scenario** | Fire evacuation scenario — 3-party liability chain |
| 6 | **Human-in-the-Loop Analysis** | HITL flow diagram + 3 failure modes + Art.14(5) two-person rule |
| 7 | **Stakeholder Map** | Plotly power-vs-impact bubble chart (8 stakeholders, hover detail) |
| 8 | **Risk Register RAG + L×I Matrix** | ISO 31000 methodology · 6 risks · heatmap + severity bar |
| 9 | **Compliance Knowledge Graph** | pyvis interactive graph · 15 nodes · 27 labelled edges · centrality sizing |
| 10 | **Reflective Commentary** | Three reflections on lab accuracy, Bridges, and cross-cutting accountability |
| 11 | **Executive Dashboard + KPIs** | Plotly gauge indicators · obligation priority bars · P1 action plan |

---

## Legal Instruments Covered

| Instrument | Application |
|-----------|-------------|
| EU AI Act (2024/1689) Art. 5(1)(h) | Potential prohibition — publicly accessible space |
| EU AI Act Annex III Pt. 1 | Automatic HIGH RISK classification — biometric ID |
| EU AI Act Arts. 9–16, 26 | All mandatory high-risk obligations |
| UK GDPR Art. 9 | Special category biometric data — lawful basis |
| UK GDPR Art. 22 | Right not to be subject to solely automated decisions |
| Equality Act 2010 s. 19 | Indirect discrimination via proxy variables |
| Equality Act 2010 s. 20 | Duty to make reasonable adjustments |
| RRO 2005 Arts. 4, 32 | Fire safety — responsible person duties |
| FCA Consumer Duty PS22/9 | Good outcomes for retail customers |
| R (Bridges) v CC South Wales [2020] | UK case law — DPIA + equality compliance required |
| PoFA 2012 / Surveillance Camera Code | Surveillance proportionality |
| NIS2 (EU) 2022/2555 | Cybersecurity obligations |

---

## Key Findings

| Finding | Detail |
|---------|--------|
| **EU AI Act classification** | HIGH RISK (Annex III Pt.1) + potential BAN (Art.5(1)(h)) |
| **Article gaps** | 11 of 13 assessed articles have compliance gaps |
| **Critical risks** | 3 risks scoring ≥16 on L×I scale |
| **Demographic bias** | NIST (2019): error rates up to 4× higher for Black women |
| **Human oversight** | Art.14(5) two-person verification rule not implemented |
| **Fire safety** | RRO 2005 integration with alarm system not tested |
| **Max ICO penalty** | Up to £17.5M or 4% global turnover |
| **EU AI Act deadline** | August 2026 |

---

## How to Run

### Google Colab (recommended — no installation needed)

1. Click the **Open in Colab** badge above  
2. `Runtime → Run All`  
3. All 11 modules render automatically

### Local Jupyter

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPO.git
cd YOUR-REPO
pip install -r requirements.txt
jupyter notebook AI_Facial_Recognition_Compliance_Explorer.ipynb
```

### Dependencies

```
plotly>=5.18.0
pandas>=2.0.0
networkx>=3.2.0
pyvis>=0.3.2
ipython>=8.0.0
```

---

## Repository Structure

```
.
├── AI_Facial_Recognition_Compliance_Explorer.ipynb   # Main notebook
├── requirements.txt                                   # Python dependencies
└── README.md                                          # This file
```

The compliance graph is saved as `compliance_graph.html` when Module 9 runs (generated at runtime, not committed).

---

## Compliance Graph — How to Read It

The Module 9 pyvis knowledge graph connects all legal nodes by relationship type:

| Edge Label | Meaning |
|-----------|---------|
| `TRIGGERS` | Annex III classification activates this obligation |
| `REQUIRES` | Article A must be satisfied before Article B |
| `ALIGNS WITH` | EU AI Act article mirrors a UK law provision |
| `ENABLES` | Compliance with A makes compliance with B achievable |
| `IMPLEMENTS` | Deployer duty implements the provider obligation |
| `RESPONSIBLE` | Vendor bears primary responsibility for this obligation |
| `INFORMS` | Article A provides evidence for Article B risk management |

**Node size = degree centrality** — bigger nodes have more connections and represent higher governance risk. Art.14 (Human Oversight) and AnnexIII are consistently the most central nodes.

---

## Legal References

- European Parliament and Council. (2024). *Regulation (EU) 2024/1689 — EU AI Act*. OJ L, 12 July 2024.
- R (Bridges) v Chief Constable of South Wales Police [2020] EWCA Civ 1058.
- Information Commissioner's Office. (2023). *Facial recognition technology: guidance for organisations*.
- Buolamwini, J. and Gebru, T. (2018). Gender Shades: Intersectional accuracy disparities in commercial gender classification. *PMLR 81*, 1–15.
- NIST. (2019). *Face Recognition Vendor Test (FRVT) Part 3: Demographic Effects*. NISTIR 8280.
- Equality Act 2010, ss. 19, 20, 29.
- Regulatory Reform (Fire Safety) Order 2005, Arts. 4, 32.
- Data Protection Act 2018, Schedule 1.
- UK GDPR Arts. 9, 22, 35.
- FCA. (2022). *Consumer Duty* (PS22/9).

---

## Academic Context

This artefact was produced for **7CS525 Human & Legal Aspects of Cyber Security** at the University of Derby (MSc Cybersecurity 2025/26) as Component 5 — Automation Artefact.

It demonstrates the **contestability principle** of the UK AI White Paper (2023): the analysis logic is transparent, reproducible and challengeable. Modifying the `ARTICLES`, `RISKS` and `EDGES` data structures in Cell 2 would adapt the entire notebook to a different AI system deployment.

---

## Disclaimer

This notebook is produced for academic purposes. Nothing in it constitutes legal advice. All legal analysis is for educational illustration only. Compliance with the EU AI Act, UK GDPR, Equality Act 2010, and all other instruments cited should be verified with qualified legal counsel.
