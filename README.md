# **Hospitalization Hypothesis Testing**

## **Introduction**
This project explores key factors influencing hospitalization charges and reasons for hospitalization based on anonymized COVID-19 patient data from Apollo Hospitals. By leveraging statistical modeling and hypothesis testing, this analysis identifies significant variables such as smoking status, viral load, and severity levels in determining medical costs. The findings provide actionable insights for optimizing healthcare processes and improving cost management.

Apollo Hospitals, a pioneer in modern healthcare in India since 1983, aims to enhance operational efficiency, refine diagnostic protocols, and better respond to health crises like the COVID-19 pandemic. This project exemplifies the power of data-driven decision-making in healthcare.

---

## **Objective**
The project addresses the following key questions:
1. Which variables significantly predict hospitalization reasons across different regions?
2. How well do variables like viral load, smoking status, and severity level explain hospitalization charges?

---

## **Data Description**
The dataset (`apollo_data.csv`) consists of anonymized patient information with the following variables:
- **age**: Age of the patient (excluding 65+ years).
- **sex**: Gender of the patient (male/female).
- **smoker**: Smoking status (yes/no).
- **region**: Residence in one of four regions (northeast, southeast, southwest, northwest).
- **viral load**: Amount of virus in the blood.
- **severity level**: Indicator of the severity of the condition.
- **hospitalization charges**: Medical costs billed (assumed in USD).

---

## **Key Insights**
### 1. **Significance of Variables for Hospitalization Reasons**
   - **Smoking status** is the most significant factor influencing hospitalization reasons across different regions.

### 2. **Description of Hospitalization Charges**
   - **Smoking status**:
     - Non-smokers: Charges reduce by ~$30,180.
     - Smokers: Charges increase by ~$29,440.
   - **Viral load**:
     - Each unit increase raises charges by ~$2,544.
   - **Severity level**:
     - Each unit increase adds ~$1,188 to charges.

### 3. **Modeling and Results**
   - Variables like smoking status, viral load, and severity level are strongly correlated with hospitalization charges (p-values < 0.05).
   - Confidence intervals validate the robustness of these relationships.

---

## **Methods**
1. **Data Preprocessing**:
   - Removed unnecessary columns.
   - Encoded categorical variables (e.g., gender, smoking status, and region) as dummy variables.
2. **Statistical Modeling**:
   - Implemented Ordinary Least Squares (OLS) regression to evaluate variable significance and correlations.
3. **Hypothesis Testing**:
   - Analyzed coefficients and confidence intervals to derive insights.

---

## **Conclusion**
This analysis demonstrates how data science can optimize healthcare management by identifying cost-driving factors. The insights can guide Apollo Hospitals in refining diagnostic and treatment protocols while maintaining affordability.


