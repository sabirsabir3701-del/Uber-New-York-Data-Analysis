# 🚖 Uber Trip Analysis – Machine Learning Project

## 📌 Project Overview
This project analyzes **Uber trip data in New York City** and builds machine learning models to **predict daily trip demand**.  
Using datasets from the NYC Taxi & Limousine Commission (TLC), we explore trends, patterns, and apply predictive modeling to forecast Uber demand.

---

## 📊 Dataset
The dataset used is **Uber-Jan-Feb-FOIL.csv** provided by TLC & FiveThirtyEight.  
It contains aggregated **daily Uber trips** along with active vehicles.

- **Columns:**
  - `date` → Date of trips  
  - `active_vehicles` → Number of active Uber vehicles that day  
  - `trips` → Total number of trips  

---

## ⚙️ Tech Stack
- **Language:** Python  
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, XGBoost  
- **Environment:** Google Colab / Jupyter Notebook  
- **Domain:** Data Analytics & Machine Learning  

---

## 🔑 Project Workflow
1. **Data Preprocessing**  
   - Convert `date` to datetime  
   - Extract features: day, day of week, month  

2. **Exploratory Data Analysis (EDA)**  
   - Trends of trips over time  
   - Average trips per weekday & month  

3. **Feature Engineering**  
   - Inputs: active vehicles, day, day of week, month  
   - Target: number of trips  

4. **Model Building**  
   - Random Forest Regressor  
   - XGBoost Regressor  
   - Gradient Boosted Trees  

5. **Model Evaluation**  
   - Metrics: R², MAPE  
   - Compare actual vs predicted trips  

6. **Visualization**  
   - Plot daily trips over time  
   - Actual vs Predicted comparison  

---

## 📈 Results
- **XGBoost** provided the best performance with the lowest MAPE.  
- Daily trip demand shows **weekly seasonality** (weekends higher).  
- Trips are strongly correlated with the number of active vehicles.  

---

## 📷 Sample Visualizations
- Trips per day over time  
- Average trips by weekday  
- Model predictions vs actual trips  

---

## 🚀 How to Run
### Option 1: Google Colab
1. Open [Google Colab](https://colab.research.google.com/)  
2. Upload the dataset (`Uber-Jan-Feb-FOIL.csv`)  
3. Run the notebook step by step  

### Option 2: Local (Jupyter Notebook / VS Code)
```bash
git clone https://github.com/your-username/uber-trip-analysis.git
cd uber-trip-analysis
pip install -r requirements.txt
jupyter notebook
