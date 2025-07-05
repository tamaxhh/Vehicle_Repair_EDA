# Vehicle Repair Data - Exploratory Data Analysis

This repository contains an Exploratory Data Analysis (EDA) of a vehicle repair dataset. The analysis aims to uncover significant patterns, assess data quality, and derive actionable insights related to vehicle maintenance and common repair issues.

## Project Overview

This project delves into a dataset detailing various aspects of vehicle repairs, customer complaints, and vehicle specifications. The core objectives of this EDA were:

* To understand the structure and characteristics of the vehicle repair data.
* To identify and address data quality issues, such as missing values.
* To uncover prevalent repair types, causal parts, and cost distributions through statistical analysis and visualizations.
* To extract key themes and insights from unstructured text data (customer complaints and repair descriptions) using text analysis techniques.
* To provide actionable recommendations based on the analytical findings.

## Data Source

The analysis was performed on a dataset containing 100 entries across 52 columns. Key columns include:
* `VIN`: Unique Vehicle Identification Number.
* `TRANSACTION_ID`: Unique identifier for each repair transaction.
* `CUSTOMER_VERBATIM` & `CORRECTION_VERBATIM`: Unstructured text describing customer complaints and repair actions.
* `CAUSAL_PART_NM`: The part identified as the cause of the issue.
* `GLOBAL_LABOR_CODE_DESCRIPTION`: Description of the labor performed.
* `TOTALCOST`: The total cost associated with the repair.
* `PLATFORM`: Vehicle platform details.

## Key Findings & Insights

1.  **Predominance of Steering Issues:** Analysis consistently highlighted "Steering Wheel Replacement" as a very common repair type. This suggests a potential recurring issue with steering systems across various models.
2.  **Variability in Repair Costs:** While most repairs fall within a typical cost range, a few instances recorded significantly higher costs, indicating complex or severe failures that warrant further investigation.
3.  **Data Quality Management:** Missing values in critical columns like `CAUSAL_PART_NM` and `TOTALCOST` were addressed through imputation (mode for categorical, mean for numerical), ensuring data completeness for robust analysis.
4.  **Value of Unstructured Data:** Textual fields (`CUSTOMER_VERBATIM`, `CORRECTION_VERBATIM`) were instrumental. Through text processing and tag generation, we were able to distil common themes and keywords related to components (e.g., 'wheel', 'engine') and conditions (e.g., 'noise', 'leak'), providing deeper insights beyond structured data.
5.  **Diverse Vehicle Population:** The dataset covers vehicles with varying mileage (`KM`) and age (`REPAIR_AGE`), suggesting that repair issues are not limited to a specific vehicle lifecycle stage.

## Recommendations

Based on the insights gained, the following recommendations are put forth:

* **Deep Dive into Steering System Failures:** Conduct further engineering analysis into the root causes of recurring steering-related issues to identify specific design or manufacturing improvements.
* **Investigate High-Cost Incidents:** Analyze the factors contributing to exceptionally high repair costs to identify systemic inefficiencies, particularly complex repair scenarios, or critical component failures.
* **Leverage Verbatim for Early Warning:** Continue to analyze customer and correction verbatim to identify emerging patterns or subtle issues that might not yet be captured by structured codes, enabling proactive interventions.
* **Tailored Maintenance Strategies:** Utilize insights on platform-specific issues and cost distributions to develop more targeted maintenance schedules and service strategies.

## Files in this Repository

* `Assessment_EDA.ipynb`: The Jupyter Notebook containing the full Exploratory Data Analysis, including data loading, cleaning, detailed column analysis, visualizations, text processing for tag generation, and comprehensive insights.

## How to Run the Notebook

To run the `Assessment_EDA.ipynb` notebook:

1.  **Clone the Repository:**
    ```bash
    git clone # Vehicle Repair Data - Exploratory Data Analysis

This repository contains an Exploratory Data Analysis (EDA) of a vehicle repair dataset. The analysis aims to uncover significant patterns, assess data quality, and derive actionable insights related to vehicle maintenance and common repair issues.

## Project Overview

This project delves into a dataset detailing various aspects of vehicle repairs, customer complaints, and vehicle specifications. The core objectives of this EDA were:

* To understand the structure and characteristics of the vehicle repair data.
* To identify and address data quality issues, such as missing values.
* To uncover prevalent repair types, causal parts, and cost distributions through statistical analysis and visualizations.
* To extract key themes and insights from unstructured text data (customer complaints and repair descriptions) using text analysis techniques.
* To provide actionable recommendations based on the analytical findings.

## Data Source

The analysis was performed on a dataset containing 100 entries across 52 columns. Key columns include:
* `VIN`: Unique Vehicle Identification Number.
* `TRANSACTION_ID`: Unique identifier for each repair transaction.
* `CUSTOMER_VERBATIM` & `CORRECTION_VERBATIM`: Unstructured text describing customer complaints and repair actions.
* `CAUSAL_PART_NM`: The part identified as the cause of the issue.
* `GLOBAL_LABOR_CODE_DESCRIPTION`: Description of the labor performed.
* `TOTALCOST`: The total cost associated with the repair.
* `PLATFORM`: Vehicle platform details.

## Key Findings & Insights

1.  **Predominance of Steering Issues:** Analysis consistently highlighted "Steering Wheel Replacement" as a very common repair type. This suggests a potential recurring issue with steering systems across various models.
2.  **Variability in Repair Costs:** While most repairs fall within a typical cost range, a few instances recorded significantly higher costs, indicating complex or severe failures that warrant further investigation.
3.  **Data Quality Management:** Missing values in critical columns like `CAUSAL_PART_NM` and `TOTALCOST` were addressed through imputation (mode for categorical, mean for numerical), ensuring data completeness for robust analysis.
4.  **Value of Unstructured Data:** Textual fields (`CUSTOMER_VERBATIM`, `CORRECTION_VERBATIM`) were instrumental. Through text processing and tag generation, we were able to distil common themes and keywords related to components (e.g., 'wheel', 'engine') and conditions (e.g., 'noise', 'leak'), providing deeper insights beyond structured data.
5.  **Diverse Vehicle Population:** The dataset covers vehicles with varying mileage (`KM`) and age (`REPAIR_AGE`), suggesting that repair issues are not limited to a specific vehicle lifecycle stage.

## Recommendations

Based on the insights gained, the following recommendations are put forth:

* **Deep Dive into Steering System Failures:** Conduct further engineering analysis into the root causes of recurring steering-related issues to identify specific design or manufacturing improvements.
* **Investigate High-Cost Incidents:** Analyze the factors contributing to exceptionally high repair costs to identify systemic inefficiencies, particularly complex repair scenarios, or critical component failures.
* **Leverage Verbatim for Early Warning:** Continue to analyze customer and correction verbatim to identify emerging patterns or subtle issues that might not yet be captured by structured codes, enabling proactive interventions.
* **Tailored Maintenance Strategies:** Utilize insights on platform-specific issues and cost distributions to develop more targeted maintenance schedules and service strategies.

## Files in this Repository

* `Assessment_EDA.ipynb`: The Jupyter Notebook containing the full Exploratory Data Analysis, including data loading, cleaning, detailed column analysis, visualizations, text processing for tag generation, and comprehensive insights.

## How to Run the Notebook

To run the `Assessment_EDA.ipynb` notebook:

1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/tamaxhh/Vehicle_Repair_EDA.git
    cd https://github.com/tamaxhh/Vehicle_Repair_EDA.git
    ```
2.  **Install Dependencies:** Ensure you have Python and Jupyter installed. You might need to install specific libraries:
    ```bash
    pip install pandas numpy matplotlib seaborn nltk openpyxl
    ```
    If you encounter NLTK data download errors, you might need to run `nltk.download('stopwords')` within a Python environment.
3.  **Launch Jupyter:**
    ```bash
    jupyter notebook
    ```
4.  Open `Assessment_EDA.ipynb` in your browser.

---

This README provides a concise overview of the project. For a detailed breakdown of the analysis, please refer to the `Assessment_EDA.ipynb` notebook.
    cd [YOUR_REPOSITORY_NAME]
    ```
2.  **Install Dependencies:** Ensure you have Python and Jupyter installed. You might need to install specific libraries:
    ```bash
    pip install pandas numpy matplotlib seaborn nltk openpyxl
    ```
    If you encounter NLTK data download errors, you might need to run `nltk.download('stopwords')` within a Python environment.
3.  **Launch Jupyter:**
    ```bash
    jupyter notebook
    ```
4.  Open `Assessment_EDA.ipynb` in your browser.

---

This README provides a concise overview of the project. For a detailed breakdown of the analysis, please refer to the `Assessment_EDA.ipynb` notebook.
