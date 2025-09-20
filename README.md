# Framework_Assignment
# COVID-19 Research Papers Explorer 📊

This project explores the **CORD-19 COVID-19 research dataset** and builds a simple **Streamlit app** for interactive analysis.  
It demonstrates data cleaning, exploratory data analysis (EDA), visualization, and deployment with Streamlit.

---

## 🚀 Project Overview
- Load and clean the metadata dataset (titles, abstracts, authors, journals, dates).
- Handle missing values and create new features (e.g., word counts).
- Perform exploratory analysis:
  - Publications per year
  - Top publishing journals
  - Frequent words in paper titles
- Build an interactive **Streamlit dashboard** for exploring results.

---

## 📂 Project Structure
project/
│-- app.py # Streamlit app
│-- metadata.csv # Raw dataset (not included here, from Kaggle CORD-19)
│-- metadata_cleaned.csv # Cleaned dataset (generated after preprocessing)
│-- README.md # Project documentation
│-- report.md # Detailed analysis report (optional)

yaml
Copy code

---

## ⚙️ Installation & Setup

1. **Clone the repository** or copy the files locally.
2. Install dependencies:
   ```bash
   pip install pandas matplotlib seaborn streamlit wordcloud
Run the Streamlit app:

bash
Copy code
streamlit run app.py
📊 Findings from Data Exploration
1. Publications Over Time
The dataset contains research papers from 1980s–2022.

Research output spiked dramatically in 2020–2021:

1,637 papers in 2020

2,128 papers in 2021

This matches the global timeline of the COVID-19 pandemic.

2. Top Publishing Journals
bioRxiv, PLoS One, BMJ, and Scientific Reports published many papers.

A large fraction were listed under "Unknown" journals — likely preprints or incomplete metadata.

3. Frequent Title Keywords
Most common words in paper titles:

covid, pandemic, sars, patients, health, disease, infection

Shows strong emphasis on clinical research, public health, and pandemic response.

⚡ Challenges
Large dataset required careful filtering and efficient loading.

Many missing values (especially abstracts and journal info).

Environment setup issues (Jupyter vs. Streamlit execution).

Some packages (e.g., wordcloud) needed to be installed manually.

💡 Learning Outcomes
Cleaning and preprocessing text-heavy scientific datasets.

Generating insights with pandas + seaborn.

Building interactive visualizations in Streamlit.

Handling missing data and caching cleaned datasets for performance.
