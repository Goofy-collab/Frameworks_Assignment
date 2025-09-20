
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

