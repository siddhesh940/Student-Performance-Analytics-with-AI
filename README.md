# Student Performance Analytics with AI

Data Analytics with AI project submitted as part of the **IBM SkillsBuild Data
Analytics with AI Academic Internship Program**, conducted by BharatCares in
association with AICTE.

## Project Description

This project explores a dataset of 1,000 students' exam scores (math,
reading, writing) together with demographic and preparation-related
attributes (gender, race/ethnicity, parental level of education, lunch type,
test preparation course completion). The goals are to:

1. Perform exploratory data analysis (EDA) to understand which factors relate
   to student exam performance.
2. Engineer an `average_score` feature and a binary `Pass`/`Fail` label
   (threshold: average score ≥ 50).
3. Train a Random Forest classifier to predict pass/fail from the
   demographic and preparation attributes.
4. Translate the findings into business/educational recommendations.

## Dataset

- **Name:** Students Performance in Exams
- **Source:** [Kaggle — spscientist/students-performance-in-exams](https://www.kaggle.com/datasets/spscientist/students-performance-in-exams)
- **Rows:** 1,000
- **Columns:** `gender`, `race/ethnicity`, `parental level of education`,
  `lunch`, `test preparation course`, `math score`, `reading score`,
  `writing score`

## Technologies Used

- Python 3
- pandas, numpy — data manipulation
- matplotlib, seaborn — data visualization
- scikit-learn — machine learning (Random Forest classifier)
- Jupyter Notebook

## Project Structure

```
├── Siddhesh_StudentPerformanceAnalytics.ipynb    # Main analysis notebook
├── StudentsPerformance.csv                       # Dataset
├── requirements.txt                              # Python dependencies
└── README.md                                     # This file
```

## Setup / Run Instructions

1. Clone this repository:
   ```bash
   git clone <your-repo-url>
   cd <repo-folder>
   ```
2. (Optional) Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate   # Windows: venv\Scripts\activate
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Launch the notebook:
   ```bash
   jupyter notebook Siddhesh_StudentPerformanceAnalytics.ipynb
   ```
5. Run all cells (Cell → Run All).

## Key Findings

- Completing the **test preparation course** is associated with a noticeable
  increase in average score across all three subjects.
- Students with **standard lunch** outperform students with free/reduced
  lunch, suggesting a socio-economic effect.
- Higher **parental level of education** correlates with higher average
  scores.
- Math, reading and writing scores are strongly correlated with one another.
- A Random Forest classifier predicts pass/fail (avg score ≥ 50) from
  demographic + preparation features with **~88% accuracy** on the held-out
  test set.

## Recommendations

1. Promote and subsidize test-preparation course enrollment.
2. Provide targeted academic support for students on free/reduced lunch.
3. Offer additional mentoring for first-generation students.
4. Investigate structural causes behind pass-rate gaps across ethnicity
   groups.

## Author

Siddhesh Patil — BCA student, IBM SkillsBuild Data Analytics with AI Academic
Internship (BharatCares x AICTE), 2026.
