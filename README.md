# Statistician in the Loop – Reimagining the Statistician for the Age of AI

This repository contains materials for the keynote address titled "Statistician in the Loop – Reimagining the Statistician for the Age of AI".

## Abstract

In the era of artificial intelligence and machine learning dominance, a fundamental question emerges: what role do statisticians play when machines can perform statistical analyses? This presentation argues that rather than becoming obsolete, statisticians are evolving into an indispensable component of AI systems—the "Statistician in the Loop"—whose expertise is more critical than ever for responsible and effective AI deployment.

This keynote speech demonstrates through a multi-agent framework applied to income prediction using simulated Public Use Microdata Sample (PUMS) data how human statistical oversight transforms AI from computational tool to rigorous scientific instrument. The framework integrates four key components: a Bayesian Inference Agent for hierarchical modeling with uncertainty quantification, a Conformal Prediction Agent generating distribution-free prediction intervals with guaranteed coverage, a Statistical Feedback Agent for bias detection and assumption validation, and critically, human decision points where statisticians provide irreplaceable judgment on bias handling and uncertainty interpretation.

Beyond technical contributions, this keynote speaks to the professional identity of statisticians in the 21st century. Far from being displaced, they are repositioned as ethical stewards and co-creators of machine intelligence. As AI systems grow in influence and complexity, the demand for statistical reasoning and ethical judgment becomes not only relevant—but urgent.

## Generated summaries

[Audio] [https://notebooklm.google.com/notebook/4c1bd8d6-b1f7-4244-b393-7d5532d01a27?artifactId=0a6e7694-27ae-4bcc-9015-39ae7e08f119](https://notebooklm.google.com/notebook/4c1bd8d6-b1f7-4244-b393-7d5532d01a27?artifactId=0a6e7694-27ae-4bcc-9015-39ae7e08f119)
[Video] [https://notebooklm.google.com/notebook/4c1bd8d6-b1f7-4244-b393-7d5532d01a27?artifactId=4ee043fd-a8df-4bbe-9244-7e3f577db090](https://notebooklm.google.com/notebook/4c1bd8d6-b1f7-4244-b393-7d5532d01a27?artifactId=4ee043fd-a8df-4bbe-9244-7e3f577db090)



## Useful Sites

- [Folktables](https://github.com/socialfoundations/folktables)
- [Public Use Microdata Sample (PUMS)](https://www.census.gov/programs-surveys/acs/microdata/access.html)

## Reproducibility Instructions

To ensure that you are using the complete and correct dataset, please follow these steps. Following this order is crucial to prevent the use of synthetic data and to ensure the reproducibility of the results:

1. **Run the `california_pums_full_eda.ipynb` notebook.** This notebook will download and process the data, creating the `california_pums_2023_complete.csv` file.
2. **Run the `short_demo.ipynb` notebook.** This notebook uses the `california_pums_2023_complete.csv` file generated in the previous step to perform the analysis.
3. **Run the `multi_agents_demo.ipynb` notebook.** Choose **Option 3** for best experience. Other options are WIP.

**Global commands**  (works at any point)

**N or NEXT** → go to the next agent

**S or SKIP** → jump straight to the end

**T or TERMINATE** → stop immediately

Append N after a choice to auto-continue (e.g., B N)

Case-insensitive; short notes after your choice are fine

**Agent 1 — StatisticalFeedbackAgent (only step with a menu)**

Choose letter or word:

A / DOCUMENT — report observed gaps as findings (no constraints)

B / FAIRNESS — exclude protected attributes (SEX, RAC1P)

C / ENGINEER — add controls/interactions to mitigate bias
Examples: A, DOCUMENT N, B - prioritize fairness. N, ENGINEER

**Agent 2 — HumanStatistician (acknowledges your choice)**

Typical input: N / NEXT

**Agent 3 — BayesianInferenceAgent**

Typical input: N / NEXT
(It applies your choice from Agent 1; no menu here.)

**Agent 4 — ConformalPredictionAgent**

Typical input: N / NEXT

**Agent 5 — VisualizationAgent (code-only output)**

It returns one Python code block that saves PNGs locally and prints file paths.

Typical input: NEXT or just let it finish.

Tip: You can use **SKIP anytime to jump to the end, or TERMINATE to stop.**



