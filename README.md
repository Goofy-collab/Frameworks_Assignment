CORD-19 Data Exploration
📌 Project Description

This project explores the CORD-19 metadata dataset, which contains over 1 million COVID-19-related research papers. The goal is to analyze publication patterns, clean the dataset, and create visualizations.

The project consists of two main parts:

Data Exploration (analysis.ipynb) – Cleaning, processing, and visualization using Pandas, Matplotlib, and Seaborn.

Interactive App (app.py) – A Streamlit app that allows users to filter publications by year and explore the dataset interactively.

🚀 Features

Data cleaning: handling missing values and parsing dates.

Visualizations:

Number of publications by year.

Top journals publishing COVID-19 research.

Most common words in paper titles.

Interactive web app using Streamlit with:

Year range slider.

Dynamic plots.

Sample data preview.

📂 Project Structure
Frameworks_Assignment/
│
├── analysis.ipynb       # Data exploration and visualization notebook
├── app.py               # Streamlit app for interactive exploration
├── metadata.csv         # Dataset (not pushed to GitHub if too large)
├── README.md            # Documentation and report
└── venv/                # Virtual environment (excluded from Git)

⚙️ Installation & Setup

Clone this repository:

git clone https://github.com/your-username/your-repo.git
cd Frameworks_Assignment


Create a virtual environment and install dependencies:

python -m venv venv
source venv/bin/activate   # Mac/Linux
venv\Scripts\activate      # Windows

pip install -r requirements.txt


Add the dataset (metadata.csv) to your project folder (don’t push this to GitHub if too big).

Run the Jupyter notebook for analysis:

jupyter notebook analysis.ipynb


Run the Streamlit app:

streamlit run app.py

🛠️ Technologies Used

Python

Pandas

Matplotlib

Seaborn

Streamlit

Jupyter Notebook

# Report on CORD-19 Data Exploration

## 1. Overview

This project involved exploring the **CORD-19 metadata dataset** using Python and building an interactive web app with **Streamlit**. The goal was to gain insights into publication patterns related to COVID-19 research and provide an easy way to filter and visualize the data.

The workflow included:

* Loading and cleaning the dataset (`metadata.csv`).
* Performing exploratory data analysis (EDA) with Pandas, Matplotlib, and Seaborn.
* Creating visualizations such as publication trends and top journals.
* Building a Streamlit app for interactive exploration.

---

## 2. Findings

### a) Publications by Year

* The dataset contains research papers spanning multiple years.
* Publications significantly increased around **2020–2021**, corresponding to the outbreak and global spread of COVID-19.
* The trend shows a research surge in pandemic years compared to earlier years.

### b) Top Journals

* Journals such as *Respiratory Research*, *BMC Infectious Diseases*, and *Journal of Virology* published a high volume of COVID-19 related work.
* This highlights key outlets where pandemic-related research was concentrated.

### c) Common Words in Titles

* Frequent words include *COVID*, *infection*, *respiratory*, *coronavirus*, and *SARS*.
* These reflect the dominant research themes and areas of focus in the dataset.

---

## 3. Challenges

* **Large dataset size (1M+ rows):**
  Handling the metadata required attention to performance and memory usage.

* **Missing and inconsistent values:**
  Many fields (e.g., `doi`, `pmcid`, `journal`) had null entries, requiring cleaning and filtering.

* **Mixed data types:**
  Several columns had mixed string/number types, leading to `DtypeWarning` during import. This required setting `low_memory=False` and casting types carefully.

* **Visualization warnings:**
  Seaborn issued deprecation warnings for `palette` usage without `hue`, requiring updated syntax in future work.

---

## 4. Learning Outcomes

* Improved understanding of **data cleaning** (handling missing values, parsing dates, type conversions).
* Learned how to use **Pandas and Seaborn** for efficient exploratory data analysis.
* Gained experience building an **interactive app with Streamlit**, including sliders, charts, and dynamic filtering.
* Practiced **Git and GitHub workflows** for version control and project documentation.

