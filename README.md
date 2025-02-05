# Biostat-G2
**Work Plan for Data Analysis Project**

### **1. Data Cleaning & Preprocessing**
- **Handle Missing Values**: Identify columns with missing data (e.g., "N/A" in organization affiliations). Use imputation (mean/mode) or removal based on context.
- **Remove Duplicates**: Check for duplicate entries using Timestamp or unique identifiers.
- **Outlier Detection**:
  - **Age**: Flag entries like "91-year-old student" for verification or removal.
  - **Scale Variables**: Ensure all Likert-scale responses (1-5) are within valid ranges.
- **Data Conversion**:
  - **Time Spent**: Convert categories (e.g., "Between 2-3 hours") to numerical midpoints.
  - **Categorical Variables**: One-hot encode gender, relationship status, and social media platforms (split comma-separated values into dummy variables).
  - **Ordinal Variables**: Treat Likert-scale responses as ordinal (e.g., 1=Strongly Disagree, 5=Strongly Agree).

---

### **2. Exploratory Data Analysis (Descriptive Statistics & Visualization)**
- **Summary Statistics**:
  - Mean, median, mode, and standard deviation for numerical variables (age, time spent, scales).
  - Frequency tables for categorical variables (gender, occupation).
- **Visualizations**:
  - Histograms: Age distribution, time spent on social media.
  - Bar Charts: Gender distribution, platform usage frequency.
  - Box Plots: Distraction levels, sleep issues across groups.
  - Heatmaps: Correlation between variables (e.g., social media time vs. depression).

---

### **3. Statistical Analysis**
- **ANOVA**:
  - Compare mean distraction levels (Q12) across age groups or occupations.
  - Test if mental health metrics (Q18, Q20) differ by social media usage time.
- **Regression**:
  - **Linear Regression**: Predict daily social media time (Q8) based on demographics/platforms.
  - **Logistic Regression**: Model binary outcomes (e.g., "Do you feel restless?" Q11) using predictors like usage frequency (Q9) and validation-seeking behavior (Q17).
  - **Multiple Regression**: Analyze how multiple factors (e.g., Q9, Q10, Q15) collectively affect depression (Q18) or sleep issues (Q20).

---

### **4. Interpretation & Reporting**
- **Key Insights**: Highlight relationships between social media habits and mental health.
- **Visual Summaries**: Use plots to illustrate findings (e.g., "Higher social media time correlates with increased distraction").
- **Recommendations**: Suggest actionable steps (e.g., limiting platform usage for at-risk demographics).

