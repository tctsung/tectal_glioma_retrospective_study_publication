# Tectal Glioma Retrospective Study

This repository contains the statistical codebase for the publication: "A single-center retrospective study of tectal gliomas: clinically and radiographically heterogenous tumors". This project is a collaboration with clinicians at NYU Langone.

**Publication Status:** Submitted to *Neuro-Oncology Journal*.

**Publication Link:** [Link to publication (placeholder)]()

This study retrospectively analyzes patients with tectal gliomas to identify imaging features that predict tumor progression. The research categorizes tumors into two groups based on MRI: Group A (confined to the tectal plate) and Group B (extending into the midbrain tegmentum). The analysis reveals that tegmental involvement (Group B) is a significant predictor of tumor progression, suggesting that this anatomical distinction can help guide clinical management, from conservative observation for Group A to more aggressive intervention for Group B.

### R Scripts

*   **`data_cleaning.Rmd`**: This script handles the initial data preparation. It reads the raw dataset from an Excel file, cleans variables such as age and patient outcomes, performs dummy coding for treatment types, and processes location and pathology data. The final cleaned dataset is saved as `clean_data.rds` for use in the analysis.
*   **`analysis.Rmd`**: This script conducts the primary statistical analysis. It loads the cleaned data, performs survival analysis (including generating Kaplan-Meier plots for overall and stratified progression-free survival), creates detailed summary tables of patient and tumor characteristics, and calculates median and N-year survival rates. The outputs, including plots and tables, are saved in the `plots_and_table/` directory.
