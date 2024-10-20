# Governance Awareness Distribution Analysis

## Overview
This project aims to analyze and visualize the awareness of rangeland governance policies using survey data. The primary focus is on generating a density plot to illustrate the distribution of responses regarding awareness, utilizing polynomial regression to smooth the curve.

---
# Tools

- **Python**: The primary programming language used for data analysis and visualization.
- 
- **Pandas**: For data manipulation and analysis.
- 
- **NumPy**: For numerical operations and handling arrays.

- **Matplotlib**: For creating static, animated, and interactive visualizations.

- **Seaborn**: For enhanced data visualization with a more aesthetically pleasing style.

- **Scikit-learn**: For polynomial regression and preprocessing.
**dotenv**: For managing environment variables.

## Setup Project

1. Clone or download the project repository.
   ```bash
   git clone git@github.com:preston-56/logit-regression-governance.git
   ```
   or, if you prefer HTTPS:
   ```bash
   git clone https://github.com/preston-56/logit-regression-governance.git

   ```
2. Set up the virtual environment:
   ```bash
        cd logit-regression-governance
        python -m venv venv
        source venv/bin/activate  # On Windows use: venv\Scripts\activate
   ```

3. Install the required packages:
    ```bash
    pip install -r requirements.txt

    ```

4. Configure the .env file (create it in the root directory) with the following variables:
   ```bash
        EXCEL_FILE_PATH: Path to the Excel file containing survey data (e.g., data/Blaise.xlsx).
        SUMMARY_OUTPUT_PATH: Path where the summary results will be saved (e.g., results/).
   ```
5. Execute the main script:
   ```bash
   python3 src/logit_regression.py
   ```

# Data Processing

- Load data from an Excel file specified in the environment variable EXCEL_FILE_PATH.
- Prepare the dependent variable by mapping responses (Yes to 1, No to 0).
- Count occurrences of each response to set up for polynomial regression.
Visualization
- A Kernel Density Estimate (KDE) plot is created to show the distribution of governance awareness.
- The polynomial regression results are overlaid on the KDE plot for a smooth curve representation.
Output
-I**mage File**: `governance_awareness_distribution.png `in the `results/` directory.

- **Text file**:`polynomial_regression_summary.txt` containing the coefficients of the polynomial regression model.
---
**Conclusion**   
 - This project provides valuable insights into the awareness of rangeland governance policies through effective data visualization techniques. 
 - Future work could involve expanding the dataset and refining the analysis to uncover deeper trends.

---
Feel free to adjust any parts to better fit your project's needs!