# Healthcare_Analysis
## 📌 Problem Statement
Hospital readmissions within 30 days represent a major 
financial and operational burden costing hospitals 
billions every year. This project analyzes 25,000+ 
patient records to identify high risk patient groups 
and key clinical factors driving readmissions — 
enabling hospitals to take targeted action to reduce 
them and improve patient outcomes.

---

## 🛠️ Tools & Technologies Used

| Tool | Purpose |
|---|---|
| Python (Pandas, Seaborn, Matplotlib) | Data Cleaning & EDA |
| Power BI | Dashboard & Visual Analysis |

---

## 🔄 Project Workflow
Raw Dataset ➝ Python (Data Cleaning & EDA) ➝ Cleaned CSV ➝ Power BI (Dashboard & Analysis)

---

## 📁 Project Structure
healthcare_analysis/
│
├── data/
│   ├── hospital_readmissions.csv        
│   └── healthcare_cleaned.csv           
│
├── notebooks/
│   └── 01_healthcare_readmission_eda.ipynb  
│
├── dashboard/
│   ├── healthcare_dashboard.pbix        
│   └── screenshots/
│       ├── page1_overview.png
│       ├── page2_demographics.png
│       └── page3_clinical_insights.png
│
└── README.md

---

## 🐍 Python — Data Cleaning & EDA

### Data Cleaning Steps
- Removed duplicate records
- Handled missing values in medical_specialty column
- Converted readmitted column from Yes/No to 1/0
- Added readmitted_label column for visualization
- Grouped rare medical specialties into "Other"
- Exported cleaned dataset for Power BI

### EDA Performed
- Readmission rate by age group
- Readmission rate by diagnosis
- Hospital stay duration vs readmission
- Medications vs readmission analysis
- Emergency visits vs readmission
- Correlation heatmap of numeric features

---

## 📊 Power BI Dashboard

### Page 1 — Overview
- Total Patients: 25K
- Total Readmitted: 12K
- Readmission Rate: 47.02%
- Donut chart: Readmitted vs Not Readmitted
- Bar chart: Readmissions by Medical Specialty

### Page 2 — Patient Demographics
- Readmission Rate by Age Group
- Readmission Rate by Diagnosis
- Diabetes Medication vs Readmission
- Age and Medical Specialty Slicers

### Page 3 — Clinical Insights
- Scatter Plot: Medications vs Inpatient Visits
- Line Chart: Emergency Visits vs Readmission Rate
- Bar Chart: Total Readmitted vs Not Readmitted
- Treemap: Readmission Rate by Diagnosis

---

## 📈 Key Findings

- 🔴 Nearly 1 in 2 patients (47.02%) were readmitted within 30 days
-  Patients aged 80-90 have the highest readmission rate at 49.58%
-  Diabetes is the #1 diagnosis linked to readmissions at 53.63%
-  Patients on diabetes medication are significantly more likely to be readmitted
-  Higher emergency visit history strongly predicts future readmissions
-  Internal Medicine handles the highest number of readmission cases
-  Significant portion of patients have unrecorded medical specialties — indicating data quality gaps

---

## 💡 Recommendations

- Implement dedicated post-discharge follow-up programs for patients aged 70-90
- Create special care plans for patients with 2+ emergency visits
- Conduct medication reviews before patient discharge
- Assign disease management programs for Diabetes and Circulatory patients
- Improve data collection for medical specialties to reduce unknown records

---

## 📸 Dashboard Screenshots

### Page 1 — Overview
Dashboard page 1 [page1]

### Page 2 — Patient Demographics
!Dashboard page 2 [Page 2]

### Page 3 — Clinical Insights
!Dashboard page 3 [Page 3]
