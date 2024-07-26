# Predicting Renal Function Post Nephrectomy for Renal Masses

## Overview
This repository contains the capstone project for the course DS-GA 1017 Responsible Data Science, Spring 2024. The project, undertaken by Anna Dominic, Chen Chen, Julia Manasson, and Siri Desiraju, focuses on developing a predictive model for renal function post nephrectomy using structured and unstructured electronic health record (EHR) data. Given the sensitivity of healthcare data, the code and data are not shared publicly.

## Team Members
- Anna Dominic (amd9200@nyu.edu)
- Chen Chen (cc4865@nyu.edu)
- Julia Manasson (manasj02@nyu.edu)
- Siri Desiraju (scd4156@nyu.edu)

## Project Structure

### 1. Introduction
Kidneys are vital organs that perform a range of essential functions. The management of renal masses often requires nephrectomy, which can impair renal function. This project aims to predict short-term postoperative renal function in patients undergoing partial or radical nephrectomy using machine learning models.

### 2. Related Work
Previous studies have utilized various statistical and machine learning approaches to predict postoperative renal function, but many are limited by single-center designs, lack of detailed data, and poorly defined postoperative timeframes.

### 3. Problem Definition and Algorithm
- **Task**: Predicting postoperative renal function (eGFR or serum creatinine) two weeks after surgery using preoperative patient characteristics and surgical details.
- **Algorithm**: The project initially used Multiple Linear Regression and subsequently employed XGBoost for its superior performance. Recursive Feature Elimination (RFE) was applied to enhance feature selection.

### 4. Experimental Evaluation
- **Data**: Data were obtained from NYU Langone Health's EHR records between 2011 and 2023. Data preprocessing included handling missing values, standardizing continuous features, and one-hot encoding categorical features.
- **Methodology**: The dataset was split into training, validation, and testing sets. Models were evaluated using Mean Squared Error (MSE), R-squared, and Mean Absolute Percentage Error (MAPE).

### 5. Results
- **Model Performance**: The XGBoost models outperformed Multiple Linear Regression in both the eGFR and Cr cohorts. Feature selection via RFE further improved predictive accuracy.
- **Subgroup Analysis**: The models performed consistently well among white patients, with higher MSE and MAPE values observed for patients of color, indicating potential challenges in accurately predicting renal function for this subgroup.

### 6. Discussion
- **Model Limitations**: The model struggled with cases of significant renal function decline post-surgery. The training set underrepresented these cases, highlighting the need for a more diverse dataset.
- **Future Improvements**: Incorporating more features related to tumor characteristics, intraoperative complications, and refining the definitions of comorbid conditions could improve the model.

### 7. Conclusion
Despite the complexities of EHR data, the project successfully developed an initial predictive model for renal function post nephrectomy. With further improvements, this model has the potential to aid in selecting the most appropriate treatment strategies for patients with renal masses.

### 8. Lessons Learned
The project underscored the challenges of working with EHR data, including extensive cleaning and preprocessing requirements. It also highlighted the importance of domain knowledge in making medically relevant assumptions and decisions.

### 9. Acknowledgements
We are immensely grateful to Dr. Madhur Nayan MD PhD for his invaluable mentorship, and to Brian McFee, Assistant Professor of Music Technology and Data Science, as well as Data Science Faculty Fellows Jacopo Cirrone, Elisha Cohen, and Saadia Gabriel for their unwavering support. We also thank NYU Langone for its resources.

## Files
Due to the sensitive nature of healthcare data, the code and data used in this project are not shared publicly.

## Usage
The models and data preprocessing steps detailed in this project are intended for academic and research purposes only. Access to the data requires proper authorization from NYU Langone Health.

## Contact
For further information, please contact the team members via their provided email addresses.

