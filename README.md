# Data Analysis on The Islands

A study measuring the effect of structured running plans on submaximal oxygen uptake (VO₂) within [**The Islands**](https://islands.smp.uq.edu.au/) — a virtual human population developed by the University of Queensland for teaching experimental design, epidemiology, and statistical reasoning.

Completed for STAT 292 by Brad Kreider.

## Research Question

How do different running training plans affect subjects' submaximal VO₂ max on The Islands?

## Design

40 subjects were randomly sampled from the town of Nelson and randomly assigned to four treatment groups (one per household, to preserve independence). Each subject's VO₂ was measured before and after a one-week protocol, with change scored as `post − pre`.

| Group | Prescription |
|-------|-------------|
| Control | No running |
| Minimal | 1 km runs |
| Moderate | 5 km runs |
| Maximal | 5 km runs (daily) |

All running was done outdoors to keep the training environment consistent. One subject withdrew from the Maximal group mid-study, leaving that group with 9 participants.

## Methods

- **One-way ANOVA** to test for differences in mean VO₂ change across groups
- **Tukey's HSD** multiple comparisons to locate the differences
- Conditions (independence, normality, equal variance) checked via residual plots; analysis conducted at the 95% confidence level in **Minitab**

## Key Findings

- The ANOVA was significant: **F = 19.90**, **p ≈ 0.000**, **R² ≈ 63%**.
- The **control** group was the only one whose VO₂ change was not significantly different from zero.
- Unexpectedly, all three running groups showed a **decrease** in VO₂ rather than the anticipated increase. Tukey's test distinguished the Moderate and Maximal groups from each other, but Minimal was statistically indistinguishable from both.
- Possible explanations discussed include subject fatigue and limitations in how The Islands simulates training adaptation.

## Repository Contents

| File | Description |
|------|-------------|
| `The Islands Data Analysis Project - Brad Kreider - FINAL.pdf` | Full written report with analysis, plots, and a formal hypothesis test |
| `Islands_Study_Tracker.xlsx` | Tracking workbook: summary sheet plus per-group compliance trackers and pre/post VO₂ measurements |

## Note

The Islands is an entirely simulated population. Subjects are virtual, and the findings have no bearing outside the simulator. No IRB review applies.
