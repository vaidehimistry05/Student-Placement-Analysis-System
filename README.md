# 🎓 Student Placement Analysis

A Python-based **Student Placement Analytics System** that analyzes student academic and extracurricular data to understand placement trends and predict student placement outcomes using **Data Science and Machine Learning** techniques.

The project combines **Python programming, Pandas, NumPy, SciPy, Matplotlib, Seaborn, Plotly, and Scikit-learn** to perform statistical analysis, visualization, data management, and placement prediction.

---

## 📌 Project Overview

Student placement depends on several factors such as academic performance, CGPA, IQ, internship experience, communication skills, extracurricular activities, and completed projects.

This project analyzes these factors using a student placement dataset and provides insights into:

* 📊 Student academic performance
* 🎓 CGPA and placement relationships
* 💼 Internship experience and placement
* 🧠 IQ and placement outcomes
* 🗣️ Communication skills
* 🏆 Extracurricular performance
* 💻 Number of completed projects
* 📈 Placement statistics
* 🤖 Machine Learning-based placement prediction
* 🔍 Feature importance
* 📊 Interactive data visualizations

---

## 🎯 Objectives

The main objectives of this project are:

1. Analyze the student placement dataset.
2. Perform data cleaning and exploratory data analysis.
3. Calculate statistical measures such as mean, median, mode, variance, standard deviation, and skewness.
4. Analyze placement rates based on different student attributes.
5. Study the relationship between internship experience and placement.
6. Perform hypothesis testing using a one-sample t-test.
7. Build a Machine Learning model to predict student placement.
8. Identify important features influencing the prediction.
9. Visualize placement trends using static and interactive charts.
10. Implement basic student record management using CSV CRUD operations.

---

## 🛠️ Technologies Used

| Technology      | Purpose                                     |
| --------------- | ------------------------------------------- |
| 🐍 Python       | Core programming language                   |
| 🐼 Pandas       | Data manipulation and analysis              |
| 🔢 NumPy        | Numerical computations                      |
| 📊 Matplotlib   | Data visualization                          |
| 🎨 Seaborn      | Statistical visualization                   |
| 📈 Plotly       | Interactive visualizations                  |
| 📐 SciPy        | Statistical analysis and hypothesis testing |
| 🤖 Scikit-learn | Machine Learning                            |
| 💾 CSV          | Student data storage and CRUD               |
| 📦 Pickle       | Student record serialization                |

---

## 📂 Project Structure

```text
Student-Placement-Analysis/
│
├── Student_Placement_analysis.ipynb
├── college_student_placement_dataset.csv
├── college_student_placement_crud.csv
├── student_module.py
├── student.dat
└── README.md
```

> Some files such as `college_student_placement_crud.csv` and `student.dat` are generated while running the notebook.

---

## 🔎 Project Workflow

```text
Dataset
   ↓
Data Loading
   ↓
Data Inspection
   ↓
Data Cleaning
   ↓
Statistical Analysis
   ↓
Exploratory Data Analysis
   ↓
Visualization
   ↓
Hypothesis Testing
   ↓
Machine Learning
   ↓
Placement Prediction
   ↓
Feature Importance
   ↓
Interactive Insights
```

---

## 📊 Data Analysis

The project performs several types of analysis using Pandas and NumPy.

### Dataset Inspection

The notebook analyzes:

* Number of rows and columns
* Column names
* Data types
* Missing values
* Duplicate records
* Descriptive statistics

### Statistical Measures

The following statistical measures are calculated:

* Mean
* Median
* Mode
* Standard deviation
* Variance
* Skewness
* Percentiles

---

## 🎓 Placement Analysis

The project analyzes placement outcomes using the following features:

* IQ
* Previous Semester Result
* CGPA
* Academic Performance
* Internship Experience
* Extra-Curricular Score
* Communication Skills
* Projects Completed

Placement statistics are calculated using Pandas grouping and aggregation.

---

## 💼 Internship Experience Analysis

The project investigates the relationship between **internship experience and placement**.

An interactive Plotly bar chart is generated to visualize the placement rate for students with and without internship experience.

---

## 📈 CGPA Analysis

The project performs detailed CGPA analysis including:

* Average CGPA
* Median CGPA
* Minimum CGPA
* Standard deviation
* Variance
* 25th, 50th, and 75th percentiles
* Number of students with CGPA ≥ 8
* Placement counts across different CGPA ranges

CGPA ranges used in the analysis:

```text
4–6
6–8
8–10
```

---

## 📐 Hypothesis Testing

A **one-sample t-test** is performed using SciPy.

The analysis tests whether the average academic percentage is significantly different from **40%**.

### Hypotheses

**Null Hypothesis (H₀):**

```text
The average academic percentage is 40%.
```

**Alternative Hypothesis (H₁):**

```text
The average academic percentage is different from 40%.
```

The significance level used is:

```text
α = 0.05
```

---

## 🤖 Machine Learning

A **Random Forest Classifier** is used to predict whether a student is likely to be placed.

### Features Used

```text
IQ
Previous Semester Result
CGPA
Academic Performance
Internship Experience
Extra-Curricular Score
Communication Skills
Projects Completed
```

### Target Variable

```text
Placement
```

The placement values are converted into numerical form:

```text
Yes → 1
No  → 0
```

---

## 🧪 Model Training

The dataset is divided into:

```text
80% → Training Data
20% → Testing Data
```

The Random Forest model uses:

```text
n_estimators = 100
random_state = 42
```

The model evaluation includes:

* Accuracy
* Classification Report
* Confusion Matrix

---

## 🔍 Feature Importance

The Random Forest model is also used to determine the relative importance of the features used for placement prediction.

A feature-importance visualization is generated to help understand which attributes contribute most to the model's predictions.

---

## 🔮 Student Placement Prediction

The notebook also demonstrates prediction for a new student using sample values such as:

```text
IQ: 110
Previous Semester Result: 8.2
CGPA: 8.5
Academic Performance: 9
Internship Experience: Yes
Extra-Curricular Score: 8
Communication Skills: 9
Projects Completed: 3
```

The model provides:

* Placement prediction
* Not-placed probability
* Placed probability

> The prediction is a machine-learning output based on the dataset and should not be treated as a guarantee of an individual's actual placement outcome.

---

## 📊 Interactive Visualizations

Plotly is used to create interactive visualizations such as:

### 1. Placement Rate by Internship Experience

Shows placement rates for students based on internship experience.

### 2. Placed Students by CGPA Range

Shows the distribution of placed students across different CGPA ranges.

### 3. CGPA vs IQ

A scatter plot showing the relationship between CGPA, IQ, and placement status.

### 4. CGPA Distribution by Placement

A histogram showing CGPA distributions for placed and non-placed students.

---

## 💾 Student Data Management

The project also demonstrates Python programming concepts beyond data analysis.

### CSV CRUD Operations

The system supports:

* Create
* Read
* Update
* Delete

operations on student placement records.

### Custom Python Module

A separate `student_module.py` file is used for displaying student information.

### Exception Handling

A custom exception:

```python
InvalidStudentError
```

is implemented for validating student records.

### Pickle

Student records are stored and retrieved using Python's `pickle` module.

---

## 🚀 How to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/Student-Placement-Analysis.git
```

### 2. Open the Project

Open the project in:

* Jupyter Notebook
* Google Colab
* VS Code

### 3. Install Required Libraries

```bash
pip install pandas numpy scipy matplotlib seaborn plotly scikit-learn
```

### 4. Add the Dataset

Make sure the following dataset is available in the project directory:

```text
college_student_placement_dataset.csv
```

### 5. Run the Notebook

Open:

```text
Student_Placement_analysis.ipynb
```

and execute the cells sequentially.

---

## ☁️ Google Colab

The notebook can also be executed using Google Colab.

Upload:

```text
Student_Placement_analysis.ipynb
college_student_placement_dataset.csv
```

Then update the dataset path if required.

For example:

```python
data = pd.read_csv("college_student_placement_dataset.csv")
```

---

## 📌 Key Learning Outcomes

Through this project, the following concepts were implemented:

* Python fundamentals
* Lists, tuples, sets, and dictionaries
* Pandas DataFrames
* NumPy arrays
* Data cleaning
* Exploratory Data Analysis
* Statistical analysis
* Data visualization
* Interactive visualization
* Hypothesis testing
* CSV file handling
* CRUD operations
* Custom modules
* Exception handling
* Pickle serialization
* Machine Learning
* Random Forest Classification
* Model evaluation
* Feature importance

---

## 🔮 Future Improvements

The project can be further enhanced by adding:

* 🌐 Streamlit web dashboard
* 📊 More interactive filters
* 📱 Responsive user interface
* 🔎 Student-wise search and analysis
* 📈 Additional ML algorithms
* ⚖️ Model comparison
* 📊 ROC-AUC evaluation
* 💾 Database integration using MySQL
* 📥 Upload-your-own-dataset functionality
* 🎯 Interactive placement prediction form
* 📋 Automated student reports

---

## 👨‍💻 Author

**Vaidehi**

Computer Engineering

---

## ⭐ Acknowledgement

This project was developed as a practical implementation of **Python, Data Science, Statistics, Data Visualization, and Machine Learning concepts** using a student placement dataset.

If you found this project useful, consider giving the repository a ⭐.
