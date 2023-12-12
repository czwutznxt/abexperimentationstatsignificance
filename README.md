Statistical Significance Framework for A/B Experimentation
Overview

This repository contains a framework for performing statistical significance tests in the context of A/B experimentation. The framework guides users through the process of defining hypotheses, selecting appropriate statistical tests, calculating sample sizes, analyzing data, and interpreting results for key performance indicators (KPIs).
Detailed Steps for Statistical Significance Framework
1. Hypothesis Definition

    Null Hypothesis (H0): No difference exists between the control (constant) and experimental (pilot) groups for each KPI.
    Alternative Hypothesis (H1): A difference exists between the control and experimental groups for each KPI.

2. Statistical Test Selection

    For continuous data (e.g., Time To Execute, Billed Revenue), consider using a t-test or ANOVA (if comparing more than two groups).
    For categorical data (e.g., Cohort Satisfaction, NPSA), consider using a chi-square test or Fisher’s exact test (if sample sizes are small).

3. Sample Size Calculation

    Determine the minimum sample size needed using power analysis to detect an effect size with a given level of significance (alpha) and power (1 - beta, with beta being the Type II error rate).

4. Delta and Percent Difference Analysis

    Calculate the differences in KPIs pre- and post-intervention for both constant and pilot groups.
    Calculate the percentage differences to standardize the impact across KPIs.

5. Outlier Handling

    Use statistical methods (e.g., Z-score, IQR) to identify and remove outliers that could affect the test's validity.

6. Significance Testing

    Apply the selected statistical test to compare the constant and pilot groups.
    Adjust for multiple comparisons if necessary to control the family-wise error rate.

7. Results Interpretation

    If p-value < alpha, reject the null hypothesis and conclude that a significant difference exists.
    Consider the effect size and confidence interval to evaluate the practical significance.

8. Documentation and Replicability

    Ensure that all steps are well-documented and can be replicated for future A/B tests.

Getting Started

To use this framework, follow these steps:

    Clone this repository to your local machine.

    Install the required Python packages by running:

    bash

    pip install -r requirements.txt

    Collect baseline data before the test and follow-up data in the constant and pilot groups.

    Use the provided Python scripts to perform statistical significance tests for your specific KPIs and data.

    Interpret the results within the context of your business to determine the practical significance of any changes observed.

Contributing

Contributions are welcome! If you have suggestions, improvements, or bug fixes, please open an issue or submit a pull request.
License

This project is licensed under the MIT License.
Contact

For inquiries or assistance, please contact czwutznxt.
