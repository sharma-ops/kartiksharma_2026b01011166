# Student Performance Analysis (Sample Data Analyst Project)

A beginner-friendly data analysis project for **B.Tech 1st Year – Data Analyst** learners.
It analyses what drives first-semester marks using Python, pandas, matplotlib and seaborn.

> The dataset is **synthetic** (computer-generated). It contains no real student data.

## Business problem
The college wants to identify which factors influence student marks so mentors can support at-risk students early.

## Questions answered
1. What is the overall performance of the batch?
2. Do attendance and study hours affect marks?
3. Does performance differ by branch, gender, residence or tutoring?
4. Which students are at risk (average marks below 50)?

## Dataset
`data/raw/student_performance.csv` – 255 rows, 11 columns (Student_ID, Gender, Branch, Residence, Attendance_Pct, Study_Hours_Per_Week, Sleep_Hours, Tutoring, Maths_Marks, Physics_Marks, Programming_Marks).
The raw file intentionally has missing values, duplicates, inconsistent text and an impossible attendance value so you can practise cleaning.

## Project structure
```
ABES_DA_Student_Performance_Project/
├── data/
│   ├── raw/student_performance.csv
│   └── processed/student_performance_clean.csv
├── notebooks/student_performance_analysis.ipynb
├── images/                  (charts saved by the notebook)
├── scripts/generate_data.py (creates the synthetic dataset)
├── requirements.txt
├── .gitignore
└── README.md
```

## How to run
```bash
git clone https://github.com/<your-username>/student-performance-analysis.git
cd student-performance-analysis
pip install -r requirements.txt
jupyter notebook notebooks/student_performance_analysis.ipynb
```

## Steps followed
1. Load and inspect data  2. Clean data (duplicates, text, outliers, missing values)  3. Create new columns (Average_Marks, Result_Band, Attendance_Band)  4. Exploratory analysis with charts  5. Insights and recommendations

## Key findings (from this dataset)
- Batch average marks ≈ 64; about 6% of students are "At Risk" (average below 50).
- Attendance and study hours both show a moderate positive correlation with marks (about 0.5).
- Students with attendance above 75% score noticeably higher than those below 60%.
- Students with tutoring score slightly higher on average.

## Charts
![Overall](images/01_overall_performance.png)
![Attendance and study](images/02_attendance_study.png)
![Correlation](images/03_correlation.png)
![Groups](images/04_group_comparison.png)

## Tools
Python 3 · pandas · NumPy · matplotlib · seaborn · Jupyter Notebook · Git and GitHub

## Author
Your Name – B.Tech 1st Year, ABES (replace with your details)
