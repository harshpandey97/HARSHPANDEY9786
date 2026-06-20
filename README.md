# PowerCo Energy — Customer Churn Prediction

Exploratory data analysis aur machine learning model jo predict karta hai ki PowerCo (energy company) ke customers churn (company chhodna) karenge ya nahi.

## 📌 Problem Statement

PowerCo, ek energy provider company, apne SME (Small & Medium Enterprise) customers ka churn rate samajhna chahti hai. Goal hai ek model banana jo predict kare ki kaunse customers near future mein company chhod sakte hain, taaki proactive retention strategies apply ki ja sakein.

## 📂 Dataset

Project mein do main datasets use hue hain:

| File | Description |
|------|--------------|
| `client_data.csv` | Customer-level information — consumption, contract details, tenure, channel sales, etc. |
| `price_data.csv` | Historical energy pricing data (off-peak, mid-peak, peak prices) for each customer |

**Shape:**
- `client_data`: 14,606 rows × 26 columns
- `price_data`: 193,002 rows × 8 columns

## 🛠️ Tech Stack

- **Python**
- **Pandas** & **NumPy** — data manipulation
- **Matplotlib** & **Seaborn** — visualization
- **Scikit-learn** — model building (churn prediction)
- **Google Colab** — development environment

## 🔍 Project Workflow

1. **Data Loading** — Import `client_data` aur `price_data` CSVs
2. **Data Cleaning** — Missing values handle karna, data types fix karna, duplicates check karna
3. **Exploratory Data Analysis (EDA)** — Churn distribution, consumption patterns, pricing trends visualize karna
4. **Feature Engineering** — Price variations (mid/off-peak/peak), tenure, consumption ratios se naye features banana
5. **Data Merging** — `client_data` aur `price_data` ko merge karna (common key: customer `id`)
6. **Model Building** — Classification model (e.g., Random Forest / Logistic Regression) train karna churn predict karne ke liye
7. **Evaluation** — Accuracy, Precision, Recall, F1-score, ROC-AUC se model evaluate karna

## 📊 Key Columns (client_data)

- `id` — Unique customer identifier
- `churn` — Target variable (1 = churned, 0 = retained)
- Consumption, contract, and pricing-related features

## 🚀 How to Run

1. Repo clone karo:
   ```bash
   git clone https://github.com/harshpandey97/HARSHPANDEY9786.git
   ```
2. Notebook `powerco_energy_data_analysis.ipynb` ko Jupyter / Google Colab mein open karo
3. Required libraries install karo:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```
4. CSV files (`client_data.csv`, `price_data.csv`) ko correct path mein rakho aur cells run karo

## 📈 Results

> *(Yahan apna final model accuracy, important insights, aur churn drivers add kar sakte ho jab model train ho jaaye)*

## 🤝 Contributing

Suggestions aur improvements welcome hain — feel free to raise an issue ya PR.

## 📄 License

This project is for educational/learning purposes.
