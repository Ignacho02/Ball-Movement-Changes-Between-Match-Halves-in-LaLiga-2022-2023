# Ball-Movement Analysis – LaLiga 2022–2023

This repository contains the statistical analyses and figure generation scripts used in the study:

**“Ball-Movement Changes Between Match Halves in LaLiga 2022–2023”**

## 📊 Project Overview

The aim of this project was to examine how ball-movement dynamics change between the first and second halves of matches during the 2022–2023 LaLiga season, and whether these changes are influenced by:

* Halftime scoreline (losing, drawing, winning)
* Team competitive level (final league position groups)

The analyses include descriptive statistics, paired-sample comparisons, and linear mixed-effects models to evaluate contextual moderation effects.

---

## 🧮 Statistical Analyses

The following analyses were performed in **Python 3.12**:

* Linear Mixed-Effects Models (statsmodels)

  * Random intercept: MatchTeam
  * Fixed effects:

    * Match Half
    * Halftime Scoreline
    * Competitive Level
    * Two-way and three-way interactions
* Omnibus F-tests for interaction effects

---

## 📈 Visualisations

Figures were generated using:

* `matplotlib`
* `seaborn`

Graphs include:

* Percentage changes between halves
* Estimated second-half adaptations (H2 – H1) by scoreline and competitive level

---

## 🛠 Requirements

Main libraries used:

```python
pandas
numpy
scipy
statsmodels
matplotlib
seaborn
```

Python version: **3.12**

---

## 📄 Data Source

Tracking and event data were obtained from:

* Opta Sports
* TRACAB tracking system
* Mediacoach (LaLiga)

Due to licensing restrictions, raw data are not publicly available.

---

## 📌 Reproducibility

All statistical models and figures presented in the manuscript were generated using the scripts included in this repository. The workflow follows:

1. Data preprocessing
2. Mixed-effects modelling
3. Figure generation

