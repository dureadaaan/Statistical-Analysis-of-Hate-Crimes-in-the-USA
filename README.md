# Statistical Analysis of Hate Crimes in the USA

A Probability & Statistics course project analyzing patterns, distributions, relationships, and statistical trends in reported hate crime data from the United States.

## 📌 Overview

This project applies statistical methods to a real-world hate crime dataset to explore how variables such as **bias motivation, offense type, location, victim age, and offender/victim counts** are distributed and related.

The analysis combines:

* Descriptive statistics
* Frequency and percentage analysis
* Probability and conditional probability
* Z-score analysis and outlier identification
* Confidence intervals
* Correlation analysis
* One-sample hypothesis testing
* Simple linear regression

The project was completed as part of **PAMa267: Probability and Statistics** at the **Pakistan Institute of Engineering and Applied Sciences (PIEAS)**.

## 👥 Authors

* **Dur e Adan**
* **Tuba Islam**
* **Javeria Khan**

**Course:** PAMa267 — Probability and Statistics
**Instructor:** Dr. Aneela Zameer
**Institution:** Department of Computer and Information Sciences, PIEAS
**Date:** December 15, 2025

---

## 🎯 Objectives

The analysis was designed to investigate several questions about the hate crime data:

1. Which bias motivation occurs most frequently?
2. Which offense types are most common?
3. Which locations account for the largest proportion of reported incidents?
4. How are victims distributed by age?
5. What relationships exist between offense type and bias motivation?
6. Are there unusual or extreme incidents in terms of victim/offender counts?
7. What can confidence intervals tell us about the average number of victims?
8. Is the average number of victims in gender-based incidents statistically different from the overall average?
9. Is there a meaningful relationship between time and the average number of victims per incident?

---

## 📊 Dataset

The project used a dataset containing recorded hate crime incidents with information including:

* Bias motivation
* Offense type
* Location of the incident
* Number of victims
* Number of offenders
* Victim/offender age categories
* Temporal attributes such as day of the week

The dataset contains **296 victims/records used for the analysis**, with both categorical and numerical variables available for statistical analysis.

---

# 🔬 Analysis

## 1. Descriptive Statistics

Frequency and percentage analyses were performed for major categorical variables, including:

* Bias motivation
* Offense type
* Location

### Bias Motivation

The analysis found that:

* **Race/Ethnicity-Based bias:** 37.63%
* **Other Bias:** 22.71%
* **Sexual Orientation-Based bias:** 20%

Race/Ethnicity-Based bias represented the largest proportion among the categories examined.

### Offense Type

The most frequent offense types were:

* **Criminal Mischief:** 18.98%
* **Assault:** 17.97%

Together, these accounted for more than one-third of the incidents analyzed.

Less frequent categories included:

* Assault by Threat: 4.41%
* Other: 2.71%

### Location

The most common locations were:

* **Residence/Home:** 25.17%
* **Street/Road:** 21.81%

Among the less frequent locations were:

* Parks/Playgrounds: 2.68%
* Commercial/Office Buildings: 3.69%

---

# 👤 Victim Age Analysis

The project examined the distribution of victims by age group.

The results showed:

* **Victims over 18:** 95.86%
* **Victims under 18:** 4.14%

Within this dataset, adults therefore represented the overwhelming majority of recorded victims.

---

# 🎲 Probability Analysis

Conditional probability was used to investigate the likelihood of particular offense types given different bias motivations.

The analysis indicated that the distribution of offense types varies across bias categories.

For example, **Religion-Based incidents were concentrated largely in one offense category**, while **Gender/Gender Identity and Sexual Orientation-Based incidents showed a more distributed pattern across offense types**.

This analysis was used to explore the relationship between **bias motivation and offense type** rather than simply examining each variable independently.

---

# 📏 Z-Score and Outlier Analysis

Z-scores were calculated to standardize victim and offender counts and identify unusually extreme observations.

An incident involving **3 victims over 18** produced an approximate:

> **Z ≈ 4.91**

Since this exceeds the commonly used threshold of:

> **|Z| > 3**

the observation was identified as an extreme outlier relative to the distribution examined.

This demonstrates how standardized scores can be used to identify unusually large observations in real-world datasets.

---

# 📐 Confidence Interval Analysis

A **95% confidence interval** was calculated for the mean number of adult victims per incident.

### Parameters

* Sample mean: **1.02**
* Sample standard deviation: **0.40**
* Sample size: **295**
* Confidence level: **95%**
* Critical Z-value: **1.96**
* Margin of error: **0.05**

### Result

**95% Confidence Interval:**

> **(0.97, 1.07)**

The analysis interprets this interval as indicating that the true average number of adult victims per incident is reasonably expected to fall within this range.

---

# 🔗 Correlation Analysis

A correlation heatmap was used to examine relationships among numerical variables related to victims and offenders.

The analysis found mostly **weak correlations**, suggesting that age-related variables alone do not strongly explain the observed hate crime patterns.

A moderate positive relationship was observed between:

* Victims under 18
* Offenders under 18

This suggests that youth-related incidents in the analyzed data may involve victims and offenders from similar age groups.

Overall, the analysis indicated that factors beyond age are likely to play a larger role in the patterns observed in the dataset.

---

# 🧪 Inferential Statistical Analysis

## One-Sample t-Test: Gender-Based Hate Crimes

A one-sample t-test was performed to examine whether the mean number of victims per incident in gender-based hate crimes differed from the overall mean.

### Variables

**Response variable:**
Number of victims per hate crime incident

**Reference population:**
All hate crime incidents in the dataset

**Sample:**
Gender-based incidents, including Gender Identity and Sexual Orientation categories

### Sample

* Sample size: **n = 76**
* Mean number of victims: **1.092**

### Hypotheses

**H₀:** μ_gender = μ₀

**H₁:** μ_gender ≠ μ₀

The significance level was set at:

> **α = 0.05**

### Result

The test **failed to reject the null hypothesis**.

Therefore, based on this analysis, there was **insufficient statistical evidence to conclude that the mean number of victims per gender-based hate crime incident differs from the overall average**.

---

# 📈 Simple Linear Regression

A simple linear regression model was used to investigate whether the **average number of victims per incident changed over time**.

### Variables

**Response variable (Y):**

Average number of victims per incident per month

**Predictor variable (X):**

Time index representing consecutive months in the study period

### Model

The relationship was modeled as:

`Yₜ = β₀ + β₁t + εₜ`

where:

* **β₀** = intercept
* **β₁** = slope representing the average monthly change
* **εₜ** = random error

The regression parameters were estimated using the **least-squares method**.

### Hypotheses

**H₀:** β₁ = 0
No linear relationship between time and average victims per incident.

**H₁:** β₁ ≠ 0
A statistically significant linear relationship exists.

### Result

The regression analysis found that the **slope was not statistically significant at the 5% level**.

Therefore, the analysis did not identify a clear upward or downward linear trend in the average number of victims per incident over time.

The project concluded that **incident severity, measured through average victim counts per incident, remained relatively stable over the study period**.

---

# 🛠️ Statistical Methods Used

| Method                   | Purpose                                                                  |
| ------------------------ | ------------------------------------------------------------------------ |
| Frequency Analysis       | Examine distributions of categorical variables                           |
| Percentage Analysis      | Compare proportions across categories                                    |
| Conditional Probability  | Examine offense likelihood given bias motivation                         |
| Z-Score                  | Standardize observations and identify extreme values                     |
| Confidence Interval      | Estimate the population mean from sample data                            |
| Correlation Analysis     | Examine relationships between numerical variables                        |
| One-Sample t-Test        | Compare a subgroup mean with the overall mean                            |
| Simple Linear Regression | Examine the relationship between time and average victim count           |
| R²                       | Evaluate the proportion of variability explained by the regression model |

---

# 📌 Key Findings

The analysis produced several notable observations:

* Race/Ethnicity-Based bias represented the largest bias category in the analyzed data at **37.63%**.
* Criminal Mischief (**18.98%**) and Assault (**17.97%**) were the most frequent offense types.
* Residences/Homes (**25.17%**) and Streets/Roads (**21.81%**) were the most common reported locations.
* Adults over 18 represented **95.86%** of recorded victims in the analyzed data.
* Conditional probability analysis showed differences in offense distributions across bias categories.
* An observation involving three adult victims produced a **Z-score of approximately 4.91**, identifying it as an extreme outlier.
* The 95% confidence interval for the mean number of adult victims was **(0.97, 1.07)**.
* The one-sample t-test did not provide sufficient evidence that gender-based incidents had a different mean victim count from the overall average.
* The regression analysis did not identify a statistically significant time trend in average victims per incident.

---

# 📚 What This Project Demonstrates

This project provided practical experience in applying probability and statistical methods to a real-world dataset.

In particular, it involved:

* Working with structured real-world data
* Exploring categorical and numerical variables
* Translating questions into statistical analyses
* Applying probability concepts to observed data
* Performing descriptive statistical analysis
* Identifying statistical outliers
* Constructing confidence intervals
* Conducting hypothesis testing
* Interpreting correlation
* Building and interpreting a simple linear regression model
* Communicating statistical findings through tables and visualizations

---

## 📄 Full Report

The complete project report, including the statistical analyses, calculations, and graphical representations, is available in this repository.

**[View the full project report](./HateCrime_Report_Appended%281%29.pdf)**

---

## ⚠️ Scope and Limitations

This project was completed as a **Probability & Statistics course project** and is primarily intended to demonstrate the practical application and interpretation of statistical techniques.

The findings describe patterns in the dataset analyzed and should not automatically be interpreted as causal explanations of hate crime behavior in the broader United States population.

The analysis focuses on the variables and statistical methods covered in the project and does not attempt to establish causal relationships between the observed factors.

---

## 🧰 Tools & Concepts

**Statistical Concepts:**
Probability · Conditional Probability · Descriptive Statistics · Z-Scores · Confidence Intervals · Hypothesis Testing · t-Test · Correlation · Linear Regression · R²

**Data Analysis:**
Structured Data Analysis · Frequency Distributions · Percentage Analysis · Statistical Visualization

---

## 🗂️ Project Type

**Course Project — Probability & Statistics**

**Institution:** Pakistan Institute of Engineering and Applied Sciences (PIEAS)

**Year:** 2025
