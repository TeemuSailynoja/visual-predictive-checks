[![DOI](https://zenodo.org/badge/939910801.svg)](https://doi.org/10.5281/zenodo.19660437)

```diff
! This paper is under review on the experimental track of the Journal of Visualization and Interaction.
Authors: @TeemuSailynoja
OC: @mjskay
AE: @Fumeng-Yang
R1: @Guoziyang27
R2: TBD
R3: TBD
```

# Recommendations for visual predictive checks in Bayesian workflow

This repository contains our paper introducing current practices in visual posterior (and prior)
predictive checks (PPCs), In the article, we provide discussion on the shortcomings of some of these
commonly used visualizations and give recommendations for alternative visualization techniques.

## Repository structure:

```bash
.
├── code 
│   └── quarto  # More extended case-studies on the examples shown in the article.
│   └── R       # Implementations of custom visualizations and PIT computations.
│   └── stan    # Source code for the probabilistic models used in the examples.
├── images      # The figures used the article.
├── index.*     # The article as qmd, pdf and html.
```

# Abstract

## Introduction
A key step in the Bayesian workflow for model building is the graphical assessment of model predictions,
whether these are drawn from the prior or posterior predictive distribution.
The goal of these assessments is
to identify whether the model is a reasonable (and ideally accurate) representation of the domain
knowledge and/or observed data. Despite the key role of these visual predictive checks in a Bayesian
workflow, there is a need for more guidance for selecting, interpreting, and
diagnosing appropriate visualizations. As a visual predictive check itself can be viewed as a 
model fit to data, assessing when this model fails to represent the data is important for drawing
well-informed conclusions.

## Demonstration

We present recommendations for visual predictive checks for observations that are: continuous,
discrete, or a mixture of the two. We also discuss diagnostics to aid in the selection of visual
methods. Specifically, in the detection of an incorrect assumption of continuously-distributed data:
identifying when data is likely to be discrete or contain discrete components, detecting and estimating
possible bounds in data, and a diagnostic of the goodness-of-fit to data for density plots made
through kernel density estimates.

## Conclusion
We offer recommendations and diagnostic tools to mitigate ad-hoc decision-making in visual
predictive checks. These contributions aim to improve the robustness and interpretability of
Bayesian model criticism practices.
