# HR Analytics: Recruitment, Performance & Attrition

## 📌 Business Problem

Employee attrition can increase hiring costs, create productivity gaps, and lead to the loss of trained talent.

This project analyzes recruitment sources, employee performance, sales quota achievement, and attrition to answer a practical HR question:

> **What patterns in the available employee and recruitment data can help HR understand attrition and make better hiring and retention decisions?**

The focus is on finding meaningful patterns while avoiding conclusions that the data cannot support.

---

## 🎯 Key Questions

The analysis focuses on four questions:

1. How significant is employee attrition in the dataset?
2. Does attrition vary across recruiting sources?
3. How do employee performance and sales quota achievement compare across the workforce?
4. What can HR realistically conclude from these patterns?

---

## 🔍 Analysis Approach

The project follows a business-focused analytical workflow:

**Raw Data → Data Validation → Data Cleaning → Attrition Analysis → Recruiting Source Analysis → Performance & Quota Analysis → Business Insights → HR Recommendations**

### Data Preparation

The `attrition` field was converted into a consistent binary outcome:

* `1` → Employee left
* `0` → Employee stayed

Recruiting-source information was also reviewed for missing values rather than silently excluding those records from the analysis.

This helps ensure that the comparisons are based on a consistent definition of attrition and that data-quality limitations remain visible.

---

## 📊 Key Insights

### 1. Recruiting source alone does not explain attrition

Attrition exists across the major recruiting sources, but the differences between sources are relatively modest.

This suggests that **recruiting source should not be treated as a standalone explanation for employee turnover**.

A lower attrition rate for a particular source is a useful signal, but it does not prove that the source produces better long-term hires.

**Business takeaway:**
Recruitment channels should be evaluated using multiple outcomes such as retention, performance, hiring volume, time-to-fill, and hiring cost.

---

### 2. Search Firm shows a positive signal

Among the recorded recruiting sources, Search Firm shows a relatively lower observed attrition rate.

However, this does not automatically make it the "best" recruitment source.

The result should be treated as a signal that can be monitored and validated using additional hiring and employee outcomes.

**Business takeaway:**
HR can investigate whether this pattern continues over time before making larger recruitment investments.

---

### 3. Missing recruiting-source data limits the analysis

A significant portion of the dataset does not contain recruiting-source information.

This makes it harder to confidently compare recruitment channels across the entire workforce.

**Business takeaway:**
Consistent recruitment-source tracking would make future hiring-channel analysis more reliable.

---

### 4. Performance and quota provide workforce context

Performance ratings and sales quota achievement provide useful information about employee outcomes.

However, these metrics should not automatically be interpreted as causes of attrition.

The analysis identifies patterns and relationships, but it does not establish causation.

**Business takeaway:**
Performance and quota should be monitored alongside attrition to understand workforce outcomes more completely.

---

## 📈 Visual Analysis

The project uses focused visuals to answer specific business questions.

### Attrition Rate by Recruiting Source

Compares observed attrition rates across recruitment channels.

**Purpose:** Identify whether certain recruiting sources show noticeably different retention outcomes.

---

### Employee Count by Recruiting Source

Shows the number of employees associated with each recruiting source.

**Purpose:** Put attrition rates into sample-size context instead of looking at percentages alone.

---

### Performance Rating vs Sales Quota %

Examines the relationship between employee performance ratings and sales quota achievement.

**Purpose:** Understand whether stronger performance is associated with stronger quota outcomes.

This is interpreted as an association rather than proof of causation.

---

### Workforce KPIs

A high-level view of:

* Total employees/records
* Overall attrition rate
* Average performance rating
* Average sales quota achievement

**Purpose:** Provide a quick overview of the workforce before exploring individual relationships.

---

## 💡 HR Recommendations

### 1. Evaluate recruitment channels using multiple metrics

Recruiting sources should not be judged using attrition alone.

A stronger evaluation framework would consider:

**Retention + Performance + Hiring Volume + Time-to-Fill + Cost-per-Hire**

---

### 2. Improve recruitment-source data capture

Recruiting source should be consistently recorded for every hire.

Better data quality would allow HR to evaluate which channels are associated with stronger long-term employee outcomes.

---

### 3. Monitor promising recruitment channels

Sources showing relatively lower observed attrition can be monitored over time before increasing investment.

---

### 4. Add employee-level factors in future analysis

To better understand *why* employees leave, future analysis could incorporate:

* Tenure
* Compensation
* Job role
* Department
* Manager
* Promotion history
* Workload
* Employee engagement/satisfaction

This would help move the analysis from identifying **where attrition occurs** toward understanding **which employee factors are associated with attrition**.

---

## ⚠️ Analytical Limitations

This analysis identifies patterns in the available data, but it does not establish causation.

Therefore, the project does **not** claim that:

* One recruiting source causes higher attrition
* One recruiting source is definitively the best
* Higher performance prevents employees from leaving
* Higher quota achievement causes better retention
* Recruiting source alone can predict employee turnover

These distinctions are important when converting analytical results into HR decisions.

---

## 🏁 Final Takeaway

> **Recruiting source provides useful signals about employee retention, but it is not strong enough on its own to explain attrition. Better recruitment-source tracking and richer employee-level data can help HR make more informed hiring and retention decisions.**

---

## 🛠️ Tools & Skills

**Python | Pandas | NumPy | Matplotlib | Data Cleaning | Exploratory Data Analysis | Data Visualization | HR Analytics | Business Analysis | Insight Communication**

---

## 📂 Project Structure

```text
HR-analysis/
│
├── HR Analytics.ipynb
├── Recruitment_Data_updated.csv
└── README.md
```

---

## 📌 Project Workflow

```text
Raw HR Data
     ↓
Data Validation & Cleaning
     ↓
Attrition Definition
     ↓
Overall Attrition Analysis
     ↓
Recruiting Source Analysis
     ↓
Performance & Quota Analysis
     ↓
Business Insights
     ↓
HR Recommendations
```

---

## 👤 About the Project

This project demonstrates an end-to-end approach to exploratory data analysis — starting with raw HR data, validating the data, identifying meaningful patterns, and translating those findings into practical business recommendations.

The emphasis is on **business thinking, analytical accuracy, and clear communication of insights** rather than simply producing charts.
