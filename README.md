# DA401--Internet-Use-Final
DA401-Final

Author: Bridget Sheehy
Date: 12/15

Project Overview

This research examines demographic patterns in weekly internet use among U.S. adults to identify which populations experience higher levels of internet exposure and may therefore be more vulnerable to potential mental health impacts. Using nationally representative data from the General Social Survey (GSS) between 2000 and 2022, the analysis focuses on exposure itself rather than mental health outcomes directly. Weekly internet use hours are modeled as a count outcome to capture intensity of digital engagement. This repository contains all data, scripts, figures, and documentation used to clean the data, estimate regression models, generate predicted values, and visualize trends in internet use across demographic groups and over time.

Goals

Answer the guiding research question: Which demographics are most likely to have high levels of internet exposure, and therefore may be more vulnerable to potential mental health impacts?

Identify how internet use varies by age, sex, education, employment status, and time.

Examine whether demographic differences in internet use persist across age groups and over survey years.

Provide a foundation for future research linking internet exposure to mental health outcomes.

Project Structure

The repository is organized to ensure clarity, transparency, and reproducibility. Raw data are preserved and never overwritten, and all analysis steps are documented.

Folder descriptions:

data: Contains raw and cleaned General Social Survey datasets used in the analysis.

figures: Stores all generated plots, including predicted internet use by age and sex and predicted internet use over time by sex.

results: Contains regression output tables and any exported model summaries.

analysis (.Rmd files): R Markdown files used for data preparation, modeling, and visualization.

README.md: Project overview, structure, and documentation.

Data

The project uses publicly available data from the General Social Survey (GSS). The primary outcome variable is weekly internet use hours (wwwhr), which measures total time spent online in a typical week. Key explanatory variables include age, sex, education, race, region, employment status, and survey year. The dataset spans 2000–2022, capturing the rapid expansion of internet access and use over time.

Methods

Research design: Observational, non-experimental

Statistical approach:

Count-based regression modeling of weekly internet use hours

Poisson regression as a baseline specification

Quasi-Poisson regression to account for substantial overdispersion in internet use data

Key modeling features:

Survey year included as a categorical variable

Demographic covariates included to capture systematic differences in exposure

Interaction terms used to assess heterogeneity by sex across age and time

All models are estimated in R, and coefficient tables for both Poisson and quasi-Poisson models are reported in the appendix.

Results

The regression models indicate that internet use varies systematically across demographic groups and has increased substantially over time. Younger individuals report significantly higher levels of weekly internet use, while education, employment status, and sex further structure patterns of exposure. Predicted values illustrate how expected internet use differs across age groups and survey years for males and females. Full model results are provided in Appendix Tables A1 and A2, and predicted trends are visualized in Appendix Figures A1 and A2.

Meaning

This project contributes to the literature on digital engagement by shifting attention from mental health outcomes alone to the distribution of internet exposure across the population. By identifying which demographic groups experience higher levels of online exposure, the analysis helps clarify where potential mental health risks may be most concentrated. These insights support more targeted approaches to future research, intervention design, and public health strategies in an increasingly digital society.

Visuals

Figure A1: Predicted weekly internet use by age and sex

Figure A2: Predicted weekly internet use by survey year and sex

Tools & Libraries

R — primary programming language

tidyverse — data cleaning and manipulation

ggplot2 — data visualization

stats — Poisson and quasi-Poisson regression modeling

R Markdown — analysis documentation and reproducibility

Limitations

The analysis relies on self-reported internet use, which may be subject to recall or reporting bias. The outcome measure captures total internet use and does not distinguish between types of online activity. Additionally, the repeated cross-sectional nature of the GSS limits causal inference and prevents tracking individual changes over time. Mental health outcomes are not directly measured in this study.

Future Steps

Future research could disaggregate internet use by type of activity, such as social media, streaming, or work-related use, to better understand exposure mechanisms. Collecting new survey data with more detailed measures of online behavior could further strengthen the analysis. Linking internet exposure data to mental health outcomes would allow for more direct assessment of vulnerability and risk.
