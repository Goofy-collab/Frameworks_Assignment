# 📘 CORD-19 Data Explorer

This project is part of the **Python Frameworks Assignment**. It analyzes the [CORD-19 research dataset](https://www.kaggle.com/allen-institute-for-ai/CORD-19-research-challenge) and builds a simple **Streamlit web application** to explore COVID-19 related research papers.

---

## 🚀 Features

* Load and clean real-world research metadata (`metadata.csv`)
* Handle missing values and extract useful features (e.g., publication year)
* Perform basic analysis:

  * Number of publications per year
  * Top journals publishing COVID-19 research
  * Sample view of paper titles, authors, and journals
* Visualize insights with **Matplotlib** and **Seaborn**
* Interactive **Streamlit application**

---

## 🛠️ Installation & Setup

### 1. Clone this repository

```bash
git clone https://github.com/your-username/Frameworks_Assignment.git
cd Frameworks_Assignment
```

### 2. Create a virtual environment

```bash
python -m venv venv
```

### 3. Activate the environment

* On Windows (PowerShell):

  ```bash
  venv\Scripts\activate
  ```
* On macOS/Linux:

  ```bash
  source venv/bin/activate
  ```

### 4. Install dependencies

```bash
pip install pandas matplotlib seaborn streamlit
```

### 5. Add dataset

Download the dataset from Kaggle and place **`metadata.csv`** inside the project folder.
⚠️ Do **not** push `metadata.csv` to GitHub (it’s large). Add this to `.gitignore`.

---

## ▶️ Run the Analysis

### Jupyter Notebook Exploration

```bash
jupyter notebook analysis.ipynb
```

### Streamlit App

```bash
streamlit run app.py
```

Then open the link in your browser (usually [http://localhost:8501](http://localhost:8501)).

---

## 📊 Findings

* **Publications spiked in 2020–2021** due to the COVID-19 pandemic.
* Top journals included **The BMJ, PLOS ONE, Journal of Virology**.
* The dataset is large (\~1M rows) but provides valuable insights into global research activity.

---

## 📝 Reflection

* Learned how to handle **large datasets** with pandas.
* Faced challenges with file permissions and dataset extraction but solved them by organizing files correctly.
* Built an **interactive Streamlit app** for the first time.
* Gained practical skills in **data cleaning, visualization, and web-based presentation**.

---

## 📂 Project Structure

```
Frameworks_Assignment/
│-- analysis.ipynb   # Jupyter notebook with data exploration
│-- app.py           # Streamlit app
│-- README.md        # Documentation
│-- .gitignore       # Ignore metadata.csv and other large files
```

---

