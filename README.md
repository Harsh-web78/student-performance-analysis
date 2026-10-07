# Student Performance Analysis

Exploratory Data Analysis (EDA) of student performance using Python, Pandas, NumPy, Matplotlib and Seaborn.

This project looks at how study habits, attendance, previous scores, sleep and background factors relate to students' final scores. The goal was to practice a complete EDA workflow - from cleaning and inspecting the data to visualising patterns and summarising findings.

## Objectives

- Inspect and clean the student performance dataset
- Explore distributions and summary statistics
- Study the relationship between study hours, attendance and final scores
- Compare performance across student groups (gender, parental education, internet access)
- Visualise correlations and key patterns
- Summarise practical takeaways from the analysis

## Tech Stack

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Jupyter Notebook

## Project Structure

```text
student-performance-analysis/
├── data/
│   └── student_performance.csv
├── notebooks/
│   └── student_performance_analysis.ipynb
├── requirements.txt
├── .gitignore
└── README.md
```

## Dataset

File: `data/student_performance.csv` (200 rows)

Columns:
- `gender` - student gender
- `age` - student age
- `study_hours` - average study hours per day
- `attendance` - attendance percentage
- `parental_education` - parents' education level
- `internet_access` - internet access at home (yes/no)
- `sleep_hours` - average sleep hours per night
- `previous_score` - score in the previous assessment
- `final_score` - final assessment score (target variable)

The CSV included here is a sample dataset prepared for this project so the notebook runs directly without any extra downloads.

## How to Run

### 1. Clone the repository

```bash
git clone https://github.com/Harsh-web78/student-performance-analysis.git
cd student-performance-analysis
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Open the notebook

```bash
jupyter notebook
```

Then open `notebooks/student_performance_analysis.ipynb` and run all cells from top to bottom.

The notebook loads the data with a relative path:

```python
pd.read_csv('../data/student_performance.csv')
```

so keep the folder structure as it is for it to work.

## Analysis Covered

1. Data overview - shape, dtypes, missing values, descriptive stats
2. Distribution of final scores and study hours
3. Study hours vs final score
4. Attendance vs final score
5. Previous score vs final score
6. Group comparison by gender, parental education and internet access
7. Correlation matrix with heatmap
8. Summary of variables most associated with final score

## Key Questions Explored

1. Does attendance relate to final score?
2. Do students who study more hours perform better?
3. How strongly does previous score relate to final score?
4. Does sleep duration show any noticeable relationship with performance?
5. Which student groups have the highest average final score?

## Findings

- Previous score has the strongest association with final score.
- Study hours and attendance both show a positive trend with final scores.
- Sleep hours show only a weak relationship in this sample.
- Group averages help highlight where differences exist, but variation within groups is large, so results should be read as associations, not causation.
- Full plots and numbers are in the notebook.

## Author

Harsh Patil
