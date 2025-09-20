# CORD-19 Data Exploration

## 📌 Project Description

This project explores the **CORD-19 metadata dataset**, which contains over 1 million COVID-19-related research papers. The goal is to analyze publication patterns, clean the dataset, and create visualizations.

The project consists of two main parts:

1. **Data Exploration (analysis.ipynb)** – Cleaning, processing, and visualization using Pandas, Matplotlib, and Seaborn.
2. **Interactive App (app.py)** – A Streamlit app that allows users to filter publications by year and explore the dataset interactively.

---

## 🚀 Features

* Data cleaning: handling missing values and parsing dates.
* Visualizations:

  * Number of publications by year.
  * Top journals publishing COVID-19 research.
  * Most common words in paper titles.
* Interactive web app using **Streamlit** with:

  * Year range slider.
  * Dynamic plots.
  * Sample data preview.

---

## 📂 Project Structure

```
Frameworks_Assignment/
│
├── analysis.ipynb       # Data exploration and visualization notebook
├── app.py               # Streamlit app for interactive exploration
├── metadata.csv         # Dataset (not pushed to GitHub if too large)
├── README.md            # Documentation and report
├── gitignore           # Ignore metadata.csv and other large files
└── venv/                # Virtual environment (excluded from Git

```

---

## ⚙️ Installation & Setup

1. Clone this repository:

   ```bash
   git clone https://github.com/Goofy-collab/Frameworks_Assignment.git
   cd Frameworks_Assignment
   ```

2. Create a virtual environment and install dependencies:

   ```bash
   python -m venv venv
   source venv/bin/activate   # Mac/Linux
   venv\Scripts\activate      # Windows

   pip install -r requirements.txt
   ```

3. Add the dataset (`metadata.csv`) to your project folder (don’t push this to GitHub if too big).

4. Run the Jupyter notebook for analysis:

   ```bash
   jupyter notebook analysis.ipynb
   ```

5. Run the Streamlit app:

   ```bash
   streamlit run app.py
   ```

---

## 🛠️ Technologies Used

* Python
* Pandas
* Matplotlib
* Seaborn
* Streamlit
* Jupyter Notebook

---

# 📊 Report on Findings

## 1. Overview

This project involved exploring the **CORD-19 metadata dataset** using Python and building an interactive web app with **Streamlit**. The goal was to gain insights into publication patterns related to COVID-19 research and provide an easy way to filter and visualize the data.

---

## 2. Findings

### a) Publications by Year

* Research publications surged in **2020–2021** during the pandemic.
* Earlier years had significantly fewer publications.

### b) Top Journals

* Journals like *Respiratory Research*, *BMC Infectious Diseases*, and *Journal of Virology* published the highest number of papers.

### c) Common Words in Titles

* Frequently occurring words include *COVID*, *infection*, *respiratory*, and *coronavirus*, showing the main themes of research.

---

## 3. Challenges

* Large dataset size (1M+ rows) caused performance and memory issues.
* Many missing and inconsistent values in fields like `doi`, `journal`.
* Mixed data types led to warnings (`DtypeWarning`).
* Seaborn’s API updates led to deprecation warnings.

---

## 4. Learning Outcomes

* Gained skills in **data cleaning** and preprocessing.
* Improved **EDA skills** with Pandas and Seaborn.
* Built an **interactive dashboard** with Streamlit.
* Learned to manage projects with **Git and GitHub**.

