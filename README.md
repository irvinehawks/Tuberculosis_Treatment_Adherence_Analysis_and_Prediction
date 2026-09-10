# TB Treatment Adherence Analysis & Prediction

An open, collaborative MSc Data Analytics and Machine Learning project focused on analysing and predicting tuberculosis treatment adherence using Python, Jupyter, VS Code, Google Colab and scikit-learn.

This project is designed as a practical learning environment for aspiring **Data Analysts, Data Scientists and Machine Learning Engineers**.

Everyone is welcome to learn from the project, create a branch, experiment, improve the analysis, add models, fix issues and submit contributions.

---

# 1. Project Overview

The project investigates whether demographic, socioeconomic and treatment-related characteristics can be used to understand and predict tuberculosis treatment adherence.

The project follows a structured analytics and machine-learning workflow:

```text
Raw Data
   ↓
Data Understanding
   ↓
Data Cleaning
   ↓
Exploratory Data Analysis
   ↓
Feature Engineering
   ↓
Model-Ready Dataset
   ↓
Google Colab
   ↓
Train/Test Split
   ↓
Machine Learning Models
   ↓
Model Evaluation
   ↓
Model Explainability
   ↓
Findings
   ↓
Final Report
```

The project is intentionally structured to resemble an industry-style data project while remaining accessible to beginners.

---

# 2. Project Objectives

The main objectives are to:

1. Understand the dataset.
2. Assess data quality.
3. Clean and prepare the dataset.
4. Perform exploratory data analysis.
5. Identify meaningful patterns and relationships.
6. Engineer useful features.
7. Train machine-learning classification models.
8. Compare model performance.
9. Evaluate models using appropriate metrics.
10. Investigate model explainability.
11. Document analytical findings.
12. Practise reproducible data-science workflows.
13. Develop practical collaboration and Git/GitHub skills.

---

# 3. Learning Objectives

By working through this project, contributors should gain practical experience with:

- Python
- pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- scikit-learn
- Jupyter Notebooks
- VS Code
- Google Colab
- Data cleaning
- Exploratory Data Analysis (EDA)
- Feature engineering
- Classification
- Train/test splitting
- Logistic Regression
- Decision Trees
- Random Forest
- SVM
- Model evaluation
- Precision
- Recall
- F1-score
- ROC-AUC
- PR-AUC
- Confusion matrices
- Feature importance
- Explainable AI
- Git
- GitHub
- Branching
- Pull Requests
- Reproducible analytics

---

# 4. Important Note About the Dataset

The dataset used in this learning project is **synthetic practice data**.

It does not represent real patients and must not be treated as real clinical evidence.

The machine-learning models produced by this project are for educational purposes only.

They should not be used to make real medical decisions.

---

# 5. Repository Structure

```text
TB_Adherence_Analysis/
│
├── .venv/
│
├── data/
│   │
│   ├── raw/
│   │   └── tb_adherence_practice_raw.csv
│   │
│   ├── processed/
│   │   └── tb_adherence_clean.csv
│   │
│   └── analysis_findings/
│       ├── df_head.csv
│       ├── df_shape.txt
│       ├── df_describe.csv
│       ├── missing_values.csv
│       └── other analytical outputs
│
├── notebooks/
│   ├── 01_data_understanding.ipynb
│   ├── 02_data_cleaning.ipynb
│   ├── 03_eda.ipynb
│   ├── 04_feature_engineering.ipynb
│   ├── 05_model_training.ipynb
│   └── 06_model_evaluation.ipynb
│
├── src/
│   ├── data_cleaning.py
│   └── modelling.py
│
├── models/
│   └── tb_adherence_model.pkl
│
├── figures/
│   ├── adherence_distribution.png
│   ├── age_distribution.png
│   ├── adherence_by_employment.png
│   ├── adherence_by_side_effects.png
│   ├── correlation_matrix.png
│   ├── confusion_matrix.png
│   └── roc_curve.png
│
├── reports/
│   └── final_report.md
│
└── README.md
```

---

# 6. What Each Directory Is For

## `data/raw/`

Contains the original dataset.

The raw dataset should **not be modified**.

```text
data/raw/
└── tb_adherence_practice_raw.csv
```

Think of this as the original source data.

---

## `data/processed/`

Contains cleaned and transformed datasets.

Example:

```text
data/processed/
└── tb_adherence_clean.csv
```

A processed dataset should be created through documented transformations rather than manually edited.

---

## `data/analysis_findings/`

Contains analytical outputs such as:

```text
df_head.csv
df_shape.txt
df_describe.csv
missing_values.csv
duplicate_records.csv
model_comparison.csv
```

These files document what was discovered during analysis.

---

## `notebooks/`

Contains the project's analysis notebooks.

Each notebook has a specific purpose.

```text
01 → Data Understanding
02 → Data Cleaning
03 → Exploratory Data Analysis
04 → Feature Engineering
05 → Model Training
06 → Model Evaluation
```

Do not put the entire project into one giant notebook.

---

## `src/`

Contains reusable Python code.

For example:

```text
src/data_cleaning.py
src/modelling.py
```

As the project becomes more advanced, reusable functions should gradually move from notebooks into `src`.

---

## `models/`

Contains trained model files.

Example:

```text
models/tb_adherence_model.pkl
```

---

## `figures/`

Contains charts generated during the analysis.

Examples:

```text
figures/adherence_distribution.png
figures/adherence_by_side_effects.png
figures/correlation_matrix.png
```

---

## `reports/`

Contains the final analytical report.

Example:

```text
reports/final_report.md
```

---

# 7. Dataset Variables

The practice dataset contains:

| Variable | Description |
|---|---|
| `patient_id` | Unique patient identifier |
| `age` | Patient age |
| `sex` | Patient sex |
| `district` | Patient district |
| `employment_status` | Employment category |
| `distance_to_clinic_km` | Distance to clinic |
| `clinic_wait_time_min` | Clinic waiting time |
| `monthly_income_usd` | Approximate monthly income |
| `missed_appointments` | Number of missed appointments |
| `support_score_1_10` | Support score |
| `side_effects` | Treatment side-effect category |
| `treatment_duration_months` | Treatment duration |
| `adherent` | Treatment adherence target |

The target variable is:

```text
adherent
```

The target contains:

```text
Yes
No
```

For machine learning this will eventually be converted to:

```text
Yes → 1
No  → 0
```

---

# 8. Local Development Environment

The initial data-analysis stages are performed locally using:

```text
Windows
 ↓
Python
 ↓
VS Code
 ↓
Jupyter
 ↓
Virtual Environment
 ↓
pandas / NumPy / Matplotlib / Seaborn / scikit-learn
```

Machine-learning training will then be performed in:

```text
Google Colab
```

---

# 9. Setting Up the Project

Clone the repository:

```bash
git clone <REPOSITORY_URL>
```

Move into the project:

```bash
cd TB_Adherence_Analysis
```

Create the virtual environment:

```bash
py -m venv .venv
```

Activate it in PowerShell:

```bash
.venv\Scripts\Activate.ps1
```

Or Command Prompt:

```bash
.venv\Scripts\activate
```

Install the required packages:

```bash
python -m pip install --upgrade pip
```

```bash
python -m pip install pandas numpy matplotlib seaborn scipy scikit-learn jupyter
```

---

# 10. VS Code Setup

Open the project folder in VS Code.

Install the Microsoft:

- Python extension
- Jupyter extension

Select the project's `.venv` as the Python interpreter.

For notebooks, select the `.venv` environment as the Jupyter kernel.

---

# 11. Project Workflow

The project must be followed in sequence.

---

## Stage 1 — Data Understanding

Notebook:

```text
notebooks/01_data_understanding.ipynb
```

Objectives:

- Load the dataset.
- Inspect the first rows.
- Determine dataset dimensions.
- Inspect data types.
- Calculate descriptive statistics.
- Identify categorical variables.
- Identify missing values.
- Identify duplicates.
- Inspect the target variable.

Important outputs should be saved in:

```text
data/analysis_findings/
```

Examples:

```text
df_head.csv
df_shape.txt
df_describe.csv
missing_values.csv
duplicate_records.csv
```

---

# 12. Stage 2 — Data Cleaning

Notebook:

```text
notebooks/02_data_cleaning.ipynb
```

Tasks include:

- Investigating duplicate records.
- Removing duplicates where appropriate.
- Investigating missing values.
- Choosing an appropriate missing-value strategy.
- Checking data types.
- Checking numerical ranges.
- Checking categorical values.
- Validating the final dataset.

The cleaned dataset should be saved as:

```text
data/processed/tb_adherence_clean.csv
```

The raw dataset must remain unchanged.

---

# 13. Stage 3 — Exploratory Data Analysis

Notebook:

```text
notebooks/03_eda.ipynb
```

EDA should investigate questions such as:

- What proportion of patients are adherent?
- Is age associated with adherence?
- Is employment status associated with adherence?
- Are side effects associated with adherence?
- Is distance to the clinic associated with adherence?
- Is clinic waiting time associated with adherence?
- Are missed appointments associated with adherence?
- Is support associated with adherence?
- What relationships exist between numerical variables?

Charts should be saved into:

```text
figures/
```

Example:

```text
figures/adherence_by_side_effects.png
```

---

# 14. Stage 4 — Feature Engineering

Notebook:

```text
notebooks/04_feature_engineering.ipynb
```

Tasks may include:

- Converting the target into binary form.
- Creating meaningful derived variables.
- Creating `appointment_risk`.
- Encoding categorical variables.
- Preparing numerical variables.
- Removing identifiers that should not be used as predictors.

For example:

```text
missed_appointments
        ↓
appointment_risk
        ↓
Low
Medium
High
```

The exact rules used to create engineered variables must be documented.

---

# 15. Model-Ready Dataset

After data cleaning, EDA and feature engineering, create a model-ready dataset.

For example:

```text
data/processed/tb_adherence_model_ready.csv
```

This dataset becomes the hand-off point between the local analysis environment and Google Colab.

---

# 16. Google Colab

Machine-learning training takes place in Google Colab.

Upload:

```text
tb_adherence_model_ready.csv
```

to the Colab environment.

The Colab workflow is:

```text
Load Data
   ↓
Separate X and y
   ↓
Identify Features
   ↓
Preprocess Features
   ↓
Train/Test Split
   ↓
Train Models
   ↓
Generate Predictions
   ↓
Evaluate Models
   ↓
Explain Models
   ↓
Save Best Model
```

---

# 17. Train/Test Split

The project uses an initial:

```text
80% Training
20% Testing
```

split.

Training data is used to teach the model.

Testing data is held back and used to evaluate performance on unseen observations.

Example:

```python
X_train, X_test, y_train, y_test = train_test_split(
    X,
    y,
    test_size=0.20,
    random_state=42,
    stratify=y
)
```

---

# 18. Machine-Learning Models

The project initially evaluates:

### Logistic Regression

```text
Baseline classification model
```

### Decision Tree

```text
Tree-based classification model
```

### Random Forest

```text
Ensemble tree-based model
```

Additional models can be added later, including:

```text
SVM
XGBoost
```

Contributors adding new models should document:

- Why the model was selected.
- How it was trained.
- Hyperparameters used.
- Performance.
- Advantages.
- Limitations.

---

# 19. Model Evaluation

Models should be evaluated using more than accuracy.

The project evaluates:

```text
Accuracy
Precision
Recall
F1-score
ROC-AUC
PR-AUC
```

Confusion matrices should also be produced.

---

# 20. Model Explainability

The project initially uses:

```text
Feature Importance
```

as an explainability technique.

Later, contributors may add:

```text
SHAP
```

or other explainability approaches.

The purpose is to understand which features contribute most strongly to model predictions.

---

# 21. Reproducibility

All analysis should be reproducible.

Contributors should:

- Use fixed random seeds where appropriate.
- Document transformations.
- Avoid manually editing datasets.
- Keep raw data unchanged.
- Record important analytical decisions.
- Keep notebooks organised.
- Use meaningful filenames.
- Save generated outputs in the appropriate directories.

---

# 22. Collaboration

This repository is **open to collaboration**.

Anyone may:

- Fork the repository.
- Create a branch.
- Experiment with the project.
- Improve documentation.
- Fix errors.
- Improve code.
- Add visualisations.
- Add statistical analysis.
- Add machine-learning models.
- Improve model evaluation.
- Add explainability techniques.
- Improve the final report.
- Submit a Pull Request.

---

# 23. Branching Strategy

Do not normally work directly on the `main` branch.

Create a new branch for your work.

Example:

```bash
git checkout -b feature/improve-eda
```

Other examples:

```text
feature/add-xgboost
feature/add-shap
feature/improve-visualisations
feature/add-statistical-tests
feature/improve-readme
fix/cleaning-error
docs/update-report
```

The branch name should describe what you are doing.

---

# 24. Typical Contribution Workflow

The recommended workflow is:

```text
Fork Repository
       ↓
Clone Your Fork
       ↓
Create Branch
       ↓
Make Changes
       ↓
Run Tests / Run Notebook
       ↓
Review Changes
       ↓
Commit
       ↓
Push Branch
       ↓
Open Pull Request
       ↓
Review
       ↓
Merge
```

---

# 25. Create Your Branch

After cloning:

```bash
git checkout -b feature/my-contribution
```

For example:

```bash
git checkout -b feature/add-random-forest-analysis
```

---

# 26. Make Your Changes

Work only on the area relevant to your branch.

For example:

```text
feature/add-eda-chart
```

should primarily concern EDA.

Avoid unrelated changes in the same branch.

---

# 27. Check Your Changes

Run your notebook or relevant code.

Check that:

- Code executes.
- Files are generated correctly.
- No unexpected errors occur.
- Existing functionality still works.
- Your findings are documented.
- File paths work correctly.

---

# 28. Commit Your Changes

Check what changed:

```bash
git status
```

Add your files:

```bash
git add .
```

Commit:

```bash
git commit -m "Add adherence analysis by side effects"
```

Commit messages should describe the change.

Good:

```text
Add adherence analysis by side effects
```

```text
Fix missing value handling
```

```text
Add Random Forest evaluation
```

Avoid vague messages such as:

```text
stuff
```

```text
changes
```

```text
update
```

---

# 29. Push Your Branch

```bash
git push origin feature/my-contribution
```

Then open a Pull Request on GitHub.

---

# 30. Pull Requests

A Pull Request should explain:

### What did you change?

Example:

> Added analysis comparing adherence across side-effect categories.

### Why did you change it?

Example:

> To investigate whether treatment side effects are associated with adherence.

### How did you test it?

Example:

> Ran the EDA notebook successfully and verified the generated figure.

### What files changed?

Example:

```text
notebooks/03_eda.ipynb
figures/adherence_by_side_effects.png
```

---

# 31. Contribution Guidelines

Contributors should follow these principles.

## Do not modify the raw dataset

Do not overwrite:

```text
data/raw/tb_adherence_practice_raw.csv
```

If you identify an issue with the raw data, document it and discuss it rather than silently modifying it.

---

## Document analytical decisions

If you decide to:

- remove a variable
- create a new feature
- remove outliers
- impute missing values
- change a model parameter
- select a particular model

explain why.

---

## Do not present assumptions as facts

For example, avoid:

> Distance causes non-adherence.

Prefer:

> Distance to the clinic was associated with differences in observed adherence in this dataset.

Remember:

```text
Association ≠ Causation
```

---

# 32. Notebook Standards

Notebooks should contain clear sections.

For example:

```markdown
# Exploratory Data Analysis

## 1. Objective

## 2. Load Data

## 3. Univariate Analysis

## 4. Bivariate Analysis

## 5. Correlation Analysis

## 6. Key Findings
```

Code should be accompanied by enough explanation that another learner can understand what is happening.

---

# 33. File Naming

Use descriptive names.

Good:

```text
adherence_by_side_effects.png
correlation_matrix.png
model_comparison.csv
```

Avoid:

```text
graph1.png
finalfinal.csv
newfile2.csv
test123.csv
```

---

# 34. Data Analysis Findings

Important tables should be stored in:

```text
data/analysis_findings/
```

Examples:

```text
df_head.csv
df_shape.txt
df_describe.csv
missing_values.csv
duplicate_records.csv
model_comparison.csv
feature_importance.csv
```

Charts should normally be stored in:

```text
figures/
```

---

# 35. Google Colab Outputs

Machine-learning outputs created in Colab should be brought back into the repository where appropriate.

For example:

```text
model_comparison.csv
confusion_matrix.png
roc_curve.png
feature_importance.png
tb_adherence_model.pkl
```

These should be placed into their appropriate project directories.

---

# 36. Suggested Future Contributions

The project is intentionally open-ended.

Possible future contributions include:

### Data Analysis

- Additional EDA.
- Statistical hypothesis testing.
- Outlier analysis.
- Distribution analysis.
- Subgroup analysis.

### Machine Learning

- SVM.
- XGBoost.
- Hyperparameter tuning.
- Cross-validation.
- GridSearchCV.
- RandomizedSearchCV.
- Class imbalance techniques.

### Explainability

- SHAP.
- Partial dependence plots.
- Permutation importance.

### Engineering

- Reusable preprocessing functions.
- Better ML pipelines.
- Automated tests.
- Configuration files.
- Logging.
- Model versioning.

### Deployment

Future contributors could turn the model into:

```text
Python API
     ↓
FastAPI
     ↓
Web Application
```

or another deployment architecture.

### MLOps

Eventually the project can explore:

```text
GitHub
   ↓
Testing
   ↓
CI/CD
   ↓
Model Training
   ↓
Model Registry
   ↓
Deployment
   ↓
Monitoring
```

---

# 37. Recommended Learning Philosophy

This project is a learning environment.

Contributors are encouraged to ask:

```text
What am I doing?

Why am I doing it?

What does the output mean?

What assumptions am I making?

Can someone else reproduce my result?

What are the limitations?
```

The goal is not simply to produce the highest-performing model.

The goal is to develop the ability to:

```text
Understand Data
      ↓
Analyse Data
      ↓
Interpret Data
      ↓
Build Models
      ↓
Evaluate Models
      ↓
Communicate Findings
      ↓
Engineer Reproducible Solutions
```

---

# 38. Code of Conduct

Contributors are expected to:

- Be respectful.
- Help beginners.
- Explain rather than dismiss.
- Give constructive feedback.
- Credit other contributors.
- Avoid plagiarism.
- Respect different approaches.
- Clearly distinguish experimentation from validated results.

---

# 39. Academic Integrity

This repository is intended for learning and collaboration.

Contributors should not present another person's work as their own.

When using external:

- articles
- datasets
- research papers
- code
- libraries
- tutorials
- methodologies

provide appropriate attribution.

---

# 40. Disclaimer

This project is educational.

The dataset is synthetic.

The results are not clinical evidence.

The models must not be used for real-world diagnosis, treatment decisions or patient risk assessment.

---

# 41. Project Status

Current stage:

```text
[x] Project structure
[x] Synthetic practice dataset
[ ] Data understanding
[ ] Data cleaning
[ ] EDA
[ ] Feature engineering
[ ] Google Colab modelling
[ ] Model evaluation
[ ] Explainability
[ ] Final report
[ ] Deployment
[ ] MLOps
```

The checklist should be updated as the project progresses.

---

# 42. How to Get Started

If you are a beginner, follow this order:

```text
1. Read this README
        ↓
2. Set up Python + VS Code
        ↓
3. Create the virtual environment
        ↓
4. Open the project
        ↓
5. Start Notebook 01
        ↓
6. Understand the raw dataset
        ↓
7. Complete Notebook 02
        ↓
8. Complete EDA
        ↓
9. Complete feature engineering
        ↓
10. Export model-ready data
        ↓
11. Open Google Colab
        ↓
12. Train models
        ↓
13. Evaluate models
        ↓
14. Explain the best model
        ↓
15. Document your findings
```

Do not skip directly to modelling without understanding and preparing the data.

---

# 43. Contributing

Contributions are welcome.

If you have an idea:

1. Fork the repository.
2. Create a branch.
3. Make your changes.
4. Test your work.
5. Document your changes.
6. Commit your work.
7. Push your branch.
8. Open a Pull Request.

Small contributions are welcome.

You do not need to be an experienced data scientist to contribute.

A beginner who improves documentation, fixes a notebook error or adds a clear explanation is making a valuable contribution.

---

# 44. Final Principle

This repository is more than a machine-learning project.

It is a practical learning environment for developing the skills required to become a:

```text
Data Analyst
     ↓
Data Scientist
     ↓
Machine Learning Engineer
```

The objective is to learn the complete journey:

```text
Raw Data
   ↓
Reliable Data
   ↓
Useful Insights
   ↓
Predictive Models
   ↓
Evaluated Models
   ↓
Explainable Models
   ↓
Reproducible Systems
```

Everyone is encouraged to learn, experiment, collaborate and improve the project.