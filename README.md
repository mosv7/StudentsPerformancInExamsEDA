# Student Performance in Exams - Exploratory Data Analysis

## 📋 Project Overview

This project conducts a comprehensive **Exploratory Data Analysis (EDA)** of student exam performance across multiple subjects. The analysis examines how various demographic, socioeconomic, and personal factors influence student academic achievement in math, reading, and writing exams.

### Main Objective
Understand the influence of various factors such as economic background, personal characteristics, and social factors on student performance in exams.

## 🎯 Key Research Questions

- How can we improve student performance in each test?
- What are the major factors influencing test scores?
- How effective is the test preparation course?
- How do demographic factors (gender, ethnicity, parental education, lunch type) correlate with performance?
- What is the overall pass rate and grade distribution?

## 📊 Dataset Overview

**File:** `StudentsPerformance.csv`

### Dataset Dimensions
- **Total Records:** 1,000 students
- **Total Columns:** 8 features

### Features

| Feature | Type | Description |
|---------|------|-------------|
| `gender` | Categorical | Student's gender (male/female) |
| `race/ethnicity` | Categorical | Student's race/ethnicity group (A, B, C, D) |
| `parental level of education` | Categorical | Highest education level of parents (high school, some college, associate's, bachelor's, master's degree) |
| `lunch` | Categorical | Lunch type (standard or free/reduced) |
| `test preparation course` | Categorical | Whether student completed test prep (none/completed) |
| `math score` | Numerical | Math exam score (0-100) |
| `reading score` | Numerical | Reading exam score (0-100) |
| `writing score` | Numerical | Writing exam score (0-100) |

**Data Quality:** No missing values detected

## 📈 Analysis Sections

### 1. **Math Score Analysis**
- Distribution is normally distributed with mean around 66.09
- Pass rate (≥40): **96%** of students
- Only 7 students achieved perfect scores (100)
- 40 students failed the math exam
- Strong correlation observed between parental education and math performance

### 2. **Reading Score Analysis**
- Highest average performance among all subjects (mean: 69.17)
- Pass rate (≥40): **97.4%** of students
- Students generally perform better in reading compared to math
- Only 26 students failed reading
- Lower education backgrounds show slightly more failures

### 3. **Writing Score Analysis**
- Highest average performance (mean: 68.06)
- Pass rate (≥40): **96.8%** of students
- Most consistent performance across education levels
- Only 32 students failed writing
- 100% pass rate observed for students with master's-educated parents

### 4. **Overall Performance**
- **Overall Pass Rate (all subjects):** 94.9% of students passed all three exams
- **Failure Rate:** 5.1% (51 students) failed at least one subject
- Parental education is a strong predictor of overall success

### 5. **Grade Distribution**

Grading Scale:
- **A Grade:** ≥80% | ~20% of students
- **B Grade:** 70-79% | ~30% of students  
- **C Grade:** 60-69% | ~22% of students
- **D Grade:** 50-59% | ~12% of students
- **E Grade:** 40-49% | ~10% of students
- **F Grade:** <40% | 5.1% of students

**Key Finding:** Grades B and C comprise the majority of students (~52%), representing the average performer group.

## 🔍 Major Findings & Insights

### Parental Education Impact
- **Master's Degree Parents:** 100% pass rate, highest A-grade proportion
- **Bachelor's Degree Parents:** 96-100% pass rates across all subjects
- **Associate's Degree Parents:** Near-perfect pass rates (98.6% in math)
- **High School/Some High School:** 91-95% pass rates, most failures
- **Key Insight:** Parental education shows the strongest correlation with student performance

### Performance Ranking by Subject
1. **Writing** - Easiest (97.4% pass rate, ~68 mean score)
2. **Reading** - Medium (97.4% pass rate, ~69 mean score)
3. **Math** - Most Challenging (96% pass rate, ~66 mean score)

### Demographic Patterns
- Students from higher socioeconomic backgrounds (indicated by parental education) consistently outperform their peers
- The gap between highest and lowest education groups is approximately 9% in overall pass rates
- Even students with less educated parents achieve a strong baseline pass rate (~91%)

## 📁 File Structure

```
StudentsPerformancInExamsEDA/
├── README.md                          # Project documentation
├── EDA.ipynb                          # Main Jupyter notebook with full analysis
└── StudentsPerformance.csv            # Dataset
```

## 🛠️ Technologies & Libraries Used

- **Python 3.x**
- **pandas** - Data manipulation and analysis
- **numpy** - Numerical computations
- **matplotlib** - Static visualization
- **seaborn** - Statistical data visualization
- **Jupyter Notebook** - Interactive analysis environment

## 🚀 How to Use

### Prerequisites
```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### Running the Analysis
1. Clone or download the repository
2. Open the Jupyter notebook:
   ```bash
   jupyter notebook EDA.ipynb
   ```
3. Run all cells sequentially to reproduce the analysis

### Key Variables in Analysis
- **Pass Mark Threshold:** 40 points (for determining pass/fail status)
- **Grading Scale:** A (≥80), B (70-79), C (60-69), D (50-59), E (40-49), F (<40)

## 💡 Conclusions & Recommendations

### For Educators & Policymakers
1. **Support Lower-Performing Groups:** Focus interventions on students from less-educated family backgrounds
2. **Math Tutoring:** Math shows the lowest pass rate; consider additional math support programs
3. **Leverage Success Models:** Learn from bachelor's and master's degree family backgrounds to inform teaching strategies
4. **Test Prep Effectiveness:** Investigate correlation between test preparation course completion and improved scores

### For Students
1. Math requires more focused attention compared to reading and writing
2. Parental involvement and background education strongly influence outcomes
3. Test preparation courses may provide measurable benefits

## 📌 Notes

- All analyses assume a passing mark threshold of 40 points
- Grade distribution reflects individual subject performance aggregated into overall performance
- No missing values were found in the dataset, ensuring data quality
- Visualizations use Seaborn's dark grid theme for enhanced clarity

## 👨‍💻 Author & Maintenance

This is an educational exploratory data analysis project. For questions or improvements, feel free to contribute or modify the notebook.

---

**Last Updated:** 2026 | **Dataset Records:** 1,000 students
