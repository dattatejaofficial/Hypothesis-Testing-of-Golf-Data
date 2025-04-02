# Hypothesis Testing of Golf Data

This project aims to evaluate the impact of a new cut-resistant coating on golf balls produced by Par Inc., a leading golf equipment manufacturer. The primary objective is to determine whether the new coating affects the driving distances of the golf balls compared to the current model.

## Table of Contents

- [Overview](#overview)
- [Project Structure](#project-structure)
- [Setup Instructions](#setup-instructions)
- [Usage](#usage)
- [Extracted Insights](#extracted-insights)
- [Dependencies](#dependencies)
- [License](#license)

## Overview

Par Inc. has developed a new cut-resistant coating for its golf balls and wishes to assess its effect on driving distance. To conduct this evaluation, 40 golf balls from both the current model and the new model with the coating were tested using a mechanical hitting machine to ensure consistency. The driving distances were measured in yards.

**Key Steps in the Analysis:**

1. **Descriptive Statistics:**
   - Calculate the mean and standard deviation of driving distances for both the current and new golf ball models.
   - Visualize the distribution of driving distances using histograms and box plots to assess normality and identify potential outliers.

2. **Hypothesis Testing:**
   - **Null Hypothesis (H₀):** There is no significant difference in the mean driving distances between the current and new golf ball models.
   - **Alternative Hypothesis (H₁):** There is a significant difference in the mean driving distances between the current and new golf ball models.
   - Perform an independent two-sample t-test to compare the means of the two groups.
   - Calculate the p-value to determine the statistical significance of the observed difference.

3. **Power Analysis:**
   - Assess the statistical power of the test to determine the likelihood of detecting a true effect if it exists.
   - Calculate the required sample size to achieve a desired power level, if necessary.

## Project Structure

The repository contains the following files:

- `hypothesis-testing-of-golf-data.ipynb`: A Jupyter Notebook that performs data loading, preprocessing, exploratory data analysis, hypothesis testing, and power analysis.
- `Golf.csv`: A CSV file containing the driving distances of the golf balls from both models.

## Setup Instructions

To set up and run the project locally, follow these steps:

1. **Clone the Repository:**
   Use the following command to clone the repository to your local machine:

   ```bash
   git clone https://github.com/dattatejaofficial/Hypothesis-Testing-of-Golf-Data.git
   ```

2. **Navigate to the Project Directory:**
   Move into the project directory:

   ```bash
   cd Hypothesis-Testing-of-Golf-Data
   ```

3. **Create a Virtual Environment (optional but recommended):**
   Set up a virtual environment to manage project dependencies:

   ```bash
   python3 -m venv env
   ```

   Activate the virtual environment:

   - On Windows:
     ```bash
     .\env\Scripts\activate
     ```
   - On macOS/Linux:
     ```bash
     source env/bin/activate
     ```

4. **Install Dependencies:**
   Install the required Python packages using pip. The necessary packages are listed in the `requirements.txt` file. If `requirements.txt` is not present, you can manually install the following packages:

   ```bash
   pip install pandas scipy statsmodels matplotlib seaborn
   ```

## Usage

To run the analysis:

1. **Ensure the Virtual Environment is Activated:**
   Make sure your virtual environment is active (refer to the setup instructions above).

2. **Run the Notebook:**
   Open `hypothesis-testing-of-golf-data.ipynb` in the Jupyter interface and execute the cells sequentially to perform the analysis and visualize the results.

## Extracted Insights

The analysis of the golf ball dataset yielded the following insights:

- **Descriptive Statistics:**
  - The mean driving distance for the current model is approximately 270.3 yards, with a standard deviation of 8.75 yards.
  - The mean driving distance for the new model is approximately 267.5 yards, with a standard deviation of 9.90 yards.
  - Histograms suggest that the current model's distances are left-skewed, while the new model's distances are right-skewed.

- **Hypothesis Testing:**
  - An independent two-sample t-test resulted in a p-value greater than the 0.05 significance level, indicating insufficient evidence to reject the null hypothesis.
  - This suggests that the new coating does not significantly affect the driving distance compared to the current model.

- **Power Analysis:**
  - The test's power was calculated to be low, implying a high probability of Type II error.
  - A larger sample size of approximately 245 observations per group is recommended to achieve adequate statistical power.

## Dependencies

The project requires the following Python packages:

- `pandas`
- `scipy`
- `statsmodels`
- `matplotlib`
- `seaborn`

These dependencies are essential for data manipulation, statistical analysis, and visualization tasks.
