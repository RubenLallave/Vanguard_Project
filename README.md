# Project: Vanguard AB Testing

## Overview
This project analyzes web analytics data and performs A/B testing to evaluate user behavior, completion rates, and error rates in an online process. The analysis includes data cleaning, transformation, and statistical testing to derive insights from user interactions.

## Project Objectives
- Clean and preprocess the data by handling missing values and duplicates.
- Transform and categorize numerical values for better interpretability.
- Merge multiple datasets to create a comprehensive view of user interactions.
- Compute completion rates, error rates, and time spent at each step in the process.
- Perform statistical tests to determine the effectiveness of the A/B test variation.
- Visualize key insights for better decision-making.

## Steps in the Analysis
1. **Data Cleaning:**
   - Handling missing values in `clnt_tenure_yr`.
   - Dropping duplicates in the web datasets.
   - Converting data types where necessary.

2. **Data Transformation:**
   - Renaming columns for better readability.
   - Categorizing `client_age` into age groups.
   - Categorizing `client_tenure_years` into tenure groups.

3. **Merging Datasets:**
   - Merging demographic data with experiment data.
   - Combining web tracking datasets for a unified view.

4. **User Journey Analysis:**
   - Sorting user interactions chronologically.
   - Computing time spent on each step.
   - Detecting errors in process steps.

5. **Experiment Analysis:**
   - Computing completion rates for test vs. control groups.
   - Analyzing time spent on each step by variation.
   - Statistical testing for significance in improvement rates.

## Statistical Testing
- **Completion Rate Test:**  
  - Null Hypothesis (H₀): Test group completion rate ≥ Control group completion rate.  
  - Alternative Hypothesis (H₁): Test group completion rate < Control group completion rate.  
  - T-test applied with a significance level of 0.05.

- **Time Spent Test:**  
  - Null Hypothesis (H₀): Test group step time ≤ Control group step time.  
  - Alternative Hypothesis (H₁): Test group step time > Control group step time.  
  - T-test applied with a significance level of 0.05.

## Results
- Computed overall and variation-specific error rates.
- Identified key bottlenecks in the process through time-spent analysis.
- Conducted statistical tests to determine the effectiveness of the experiment.

## Project Management
The progress of this project is tracked using a **Kanban board** on Trello:  
[Trello Board](https://trello.com/b/uX4BQgNM/vanguard-project)

## Technologies Used
- Python (Pandas, NumPy, SciPy, Matplotlib, Seaborn)
- Jupyter Notebook
- Tableau (Data Visualization)
- Trello (Project Management)

## Data Sources
The datasets used in this project were sourced from the following links:

1. **Demographics Data:**  
   [https://raw.githubusercontent.com/data-bootcamp-v4/lessons/refs/heads/main/5_6_eda_inf_stats_tableau/project/files_for_project/df_final_demo.txt](https://raw.githubusercontent.com/data-bootcamp-v4/lessons/refs/heads/main/5_6_eda_inf_stats_tableau/project/files_for_project/df_final_demo.txt)

2. **Web Data (Part 1):**  
   [https://raw.githubusercontent.com/data-bootcamp-v4/lessons/refs/heads/main/5_6_eda_inf_stats_tableau/project/files_for_project/df_final_web_data_pt_1.txt](https://raw.githubusercontent.com/data-bootcamp-v4/lessons/refs/heads/main/5_6_eda_inf_stats_tableau/project/files_for_project/df_final_web_data_pt_1.txt)

3. **Web Data (Part 2):**  
   [https://raw.githubusercontent.com/data-bootcamp-v4/lessons/refs/heads/main/5_6_eda_inf_stats_tableau/project/files_for_project/df_final_web_data_pt_2.txt](https://raw.githubusercontent.com/data-bootcamp-v4/lessons/refs/heads/main/5_6_eda_inf_stats_tableau/project/files_for_project/df_final_web_data_pt_2.txt)

4. **Experiment Data:**  
   [https://raw.githubusercontent.com/data-bootcamp-v4/lessons/refs/heads/main/5_6_eda_inf_stats_tableau/project/files_for_project/df_final_experiment_clients.txt](https://raw.githubusercontent.com/data-bootcamp-v4/lessons/refs/heads/main/5_6_eda_inf_stats_tableau/project/files_for_project/df_final_experiment_clients.txt)

## How to Run
1. Install required libraries using:
   ```bash
   pip install pandas numpy scipy matplotlib seaborn
   ```
2. Run the Python script or Jupyter Notebook to execute the analysis.

## Contributors
- André Barros
- Rubèn Lallave Fabregat
- Rafal Kolakowski

## License
This project is for educational purposes. Feel free to use and modify it as needed.

