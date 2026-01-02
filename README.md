# IBM Applied Data Science Capstone – SpaceX Launch Analysis

This repository contains the final capstone project for the **IBM Applied Data Science Professional Certificate**.  
The project analyzes historical SpaceX Falcon 9 launch data to identify the key factors that influence **first-stage landing success**, and explores how these insights can support cost reduction strategies through reusable rockets.

---

##  Project Objectives

- Analyze historical SpaceX launch data using data science techniques  
- Identify factors affecting first-stage landing success  
- Perform exploratory data analysis (EDA) using visualization and SQL  
- Build interactive visual analytics using **Folium** and **Plotly Dash**  
- Train and evaluate **machine learning classification models** to predict landing success  

---

##  Technologies & Tools

- **Python** (Pandas, NumPy, Scikit-learn)
- **SQL** (SQLite)
- **Data Visualization**: Matplotlib, Seaborn
- **Interactive Visualization**: Folium, Plotly Dash
- **Machine Learning**: Logistic Regression, SVM, Decision Tree, KNN
- **Web Scraping**: BeautifulSoup
- **APIs**: SpaceX REST API
- **Version Control**: Git & GitHub

---

## Presentation

<a href="https://1drv.ms/p/c/ac68488bceaf3cbf/IQBRVdnovnGfQIqkuRIecw_rAWk2udAS4ZmTxCIMO3krsrU?e=yrHpwC" target="_blank">
Final Project Presentation (PDF)
</a>


---

##  Repository Structure

```text
IBM_DataScience_Capstone/
│
├── appendix/
│   └── Additional materials such as SQL queries, code snippets,
│       charts, and supporting assets referenced in the presentation
│
├── dashboard_app/
│   ├── spacex_launch_dash.csv
│   └── spacex-dash-app.py
│       # Plotly Dash application for interactive data visualization
│
├── data/
│   ├── raw/
│   │   # Data collected directly from SpaceX APIs and Wikipedia
│   │
│   └── processed/
│       ├── dataset_part_1.csv
│       ├── dataset_part_2.csv
│       └── dataset_part_3.csv
│       # Cleaned and processed datasets used for EDA and ML modeling
│
├── images/
│   └── Project-related images, diagrams, and visual assets
│
├── ml/
│   └── Machine Learning related code snippets and modeling references
│
├── notebooks/
│   ├── 01-jupyter-labs-spacex-data-collection-api.ipynb
│   ├── 02-jupyter-labs-webscraping.ipynb
│   ├── 03-labs-jupyter-spacex-data-wrangling.ipynb
│   ├── 04-jupyter-labs-eda-sql-coursera-sqlite.ipynb
│   ├── 05-jupyter-labs-eda-dataviz-v2.ipynb
│   ├── 06-lab-jupyter-launch-site-location-v2.ipynb
│   └── 07-SpaceX-Machine-Learning-Prediction-Part-5-v1.ipynb
│
├── presentation/
│   └── Final project presentation (PDF format)
│
├── requirements.txt
│   # Python dependencies
│
├── README.md
│
└── .gitignore
