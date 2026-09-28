 Student Placement Analysis System

A Python-based Student Placement Analysis System that analyzes student academic and extracurricular data, performs statistical analysis, manages student records, and uses Machine Learning to predict student placement outcomes.

📌 Project Overview

This project uses a student placement dataset containing factors such as:

IQ

Previous Semester Result

CGPA

Academic Performance

Internship Experience

Extra-Curricular Score

Communication Skills

Projects Completed

Placement Status

The notebook demonstrates Python programming, data analysis, statistics, visualization, file handling, CRUD operations, and Machine Learning in one project.

🎯 Objectives

Analyze student placement data using Pandas and NumPy.

Calculate statistical measures such as mean, median, mode, variance, standard deviation, and skewness.

Analyze placement trends based on academic and extracurricular factors.

Study placement rates according to internship experience.

Perform hypothesis testing using a one-sample t-test.

Implement student record storage using Pickle and a custom Python module.

Perform CSV-based CRUD operations.

Build a Random Forest model for placement prediction.

Evaluate the Machine Learning model using accuracy, classification report, and confusion matrix.

Analyze feature importance.

Create interactive visualizations using Plotly.

🛠️ Technologies & Libraries

Python

Pandas – data manipulation and analysis

NumPy – numerical operations

SciPy – statistical testing

Matplotlib – visualization

Seaborn – statistical visualization

Plotly – interactive visualizations

Scikit-learn – Machine Learning

CSV – student record management

Pickle – student record serialization

📊 Data Analysis

The project performs:

Dataset inspection

Row and column analysis

Data type checking

Missing-value checking

Duplicate-record checking

Descriptive statistics

Placement distribution analysis

Performance comparison by placement status

Performance comparison by internship experience

CGPA statistical analysis

CGPA percentile analysis

Statistical Measures

The notebook calculates:

Mean

Median

Mode

Standard Deviation

Variance

Skewness

25th, 50th, and 75th Percentiles

📐 Hypothesis Testing

A one-sample t-test is performed on academic percentage.

Hypotheses

H₀: The average academic percentage is 40%.

H₁: The average academic percentage is different from 40%.

The significance level used is:

α = 0.05

The result is evaluated using the calculated t-statistic and p-value.

💾 Student Record Management

The project also demonstrates Python file-handling concepts.

Pickle & Custom Module

A custom student_module.py module is created to display student details.

Student records are stored and retrieved using Python's pickle module.

A custom exception named:

InvalidStudentError

is also implemented for validation.

CSV CRUD

The project includes CSV-based:

Create – Add a new student

Read – Display student records

Update – Modify student records

Delete – Remove student records

The CRUD operations are performed on a working copy of the placement dataset.

🤖 Machine Learning

A Random Forest Classifier is used for student placement prediction.

Features

IQ
Prev_Sem_Result
CGPA
Academic_Performance
Internship_Experience
Extra_Curricular_Score
Communication_Skills
Projects_Completed

Target

Placement

Placement values are encoded as:

Yes → 1
No  → 0

Model Configuration

RandomForestClassifier(
    n_estimators=100,
    random_state=42
)

The dataset is divided into:

80% Training Data
20% Testing Data

with stratification applied to the target variable.

📈 Model Evaluation

The Random Forest model is evaluated using:

Accuracy

Accuracy Percentage

Classification Report

Confusion Matrix

A Seaborn heatmap is used to visualize the confusion matrix.

🔍 Feature Importance

The project calculates feature importance using the trained Random Forest model.

A bar chart is created to visualize the relative importance of the features used for placement prediction.

🔮 Student Placement Prediction

The notebook demonstrates prediction for a sample student using:

IQ

Previous Semester Result

CGPA

Academic Performance

Internship Experience

Extra-Curricular Score

Communication Skills

Projects Completed

The model returns:

Predicted placement status

Not-placed probability

Placed probability

Machine Learning predictions are based on the dataset and model used in this project and should not be treated as a guarantee of an individual's actual placement outcome.

📊 Interactive Visualizations

The project uses Plotly to create interactive charts.

1. Placement Rate by Internship Experience

Shows the placement rate for students with different internship experience statuses.

2. Placed Students by CGPA Range

Groups placed students into:

4–6
6–8
8–10

and displays the distribution using a pie chart.

3. CGPA vs IQ by Placement

An interactive scatter plot showing CGPA and IQ, categorized by placement status.

4. CGPA Distribution by Placement

An interactive histogram showing CGPA distribution according to placement status.

📂 Project Structure

Student-Placement-Analysis-System/
│
├── Student_Placement_analysis.ipynb
├── college_student_placement_dataset.csv
├── README.md
└── PDS CIPAT Report Format.pdf

Additional files such as student_module.py, student.dat, and the CRUD working CSV are generated when the relevant notebook cells are executed.

🚀 How to Run

1. Clone the Repository

git clone https://github.com/YOUR-USERNAME/Student-Placement-Analysis-System.git

2. Install Required Libraries

pip install pandas numpy scipy matplotlib seaborn plotly scikit-learn

3. Open the Notebook

Open:

Student_Placement_analysis.ipynb

using Jupyter Notebook, JupyterLab, Google Colab, or VS Code.

4. Dataset Path

Make sure:

college_student_placement_dataset.csv

is available in the notebook environment.

If using Google Colab, upload the dataset and run the notebook cells sequentially.

📚 Concepts Demonstrated

This project covers:

Python Variables

Lists

Tuples

Sets

Dictionaries

Functions

Exception Handling

Custom Modules

Pickle

CSV File Handling

CRUD Operations

Pandas

NumPy

Statistical Analysis

Hypothesis Testing

Data Visualization

Interactive Visualization

Machine Learning

Random Forest Classification

Model Evaluation

Feature Importance

🔮 Future Improvements

Possible future enhancements include:

Streamlit-based web dashboard

Interactive student prediction form

Database integration

Additional Machine Learning models

Model comparison

Advanced filtering and analysis

Student-wise reports

Dataset upload functionality

👩‍💻 Author

Vaidehi
Computer Engineering

⭐ If you find this project useful, consider giving the repository a star.
