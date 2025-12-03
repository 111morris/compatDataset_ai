# COMPAS Dataset Bias Analysis

This project analyzes racial bias in the COMPAS (Correctional Offender Management Profiling for Alternative Sanctions) dataset using the AI Fairness 360 (AIF360) toolkit. It explores fairness metrics, visualizes bias, and applies mitigation techniques.

## Project Overview

The COMPAS algorithm is used to assess the likelihood of a defendant becoming a recidivist. This project investigates whether the algorithm exhibits racial bias against African American defendants compared to Caucasian defendants.

Key activities include:
- Loading and preprocessing the COMPAS dataset.
- Computing fairness metrics (e.g., Mean Difference).
- Visualizing False Positive Rates by race.
- Applying the **Reweighing** algorithm to mitigate bias.
- Re-evaluating fairness metrics after mitigation.

## Files Description

- **`main.ipynb`**: The main Jupyter Notebook containing the code for data loading, analysis, visualization, and bias mitigation.
- **`compas-scores-two-years.csv`**: The raw dataset used for analysis (downloaded from ProPublica).
- **`report_summarizing_findings_and_remediation_steps.pdf`**: A detailed report summarizing the findings of the analysis and suggested remediation steps.
- **`ethical_reflection.pdf`**: A document reflecting on the ethical implications of using AI in criminal justice.

## Installation & Usage

### Prerequisites

Ensure you have Python installed along with the following libraries:
- `aif360`
- `pandas`
- `matplotlib`
- `scikit-learn`
- `numpy`

You can install them using pip:

```bash
pip install aif360 pandas matplotlib scikit-learn numpy
```

### Running the Project

1.  Clone the repository.
2.  Navigate to the project directory.
3.  Launch Jupyter Notebook:
    ```bash
    jupyter notebook
    ```
4.  Open `main.ipynb` and run the cells sequentially.

## References

- **ProPublica Analysis**: [Machine Bias](https://www.propublica.org/article/machine-bias-risk-assessments-in-criminal-sentencing)
- **AIF360**: [AI Fairness 360 Open Source Toolkit](https://aif360.mybluemix.net/)
