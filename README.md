# 📈 Cryptocurrency Anomaly Detection 

This project applies **unsupervised machine learning models** to detect unusual activities in cryptocurrency trading data. We use **Isolation Forest** and **DBSCAN** to identify anomalies in **price, trading volume, and market cap** that may indicate market manipulations or extreme fluctuations.

---

## Problem Statement  
Cryptocurrency markets experience frequent fluctuations, but some anomalies might indicate **unusual activities** such as pump-and-dump schemes, liquidity issues, or significant shifts in investor behavior.  
This project aims to **detect such anomalies using machine learning**, allowing traders and analysts to identify irregular patterns.

---

## Approach  
1. **Exploratory Data Analysis (EDA)**  
   - Visualize **distributions** of price, volume, and market cap  
   - Detect **missing values** and perform data cleaning  
   - Analyze **correlations** between different financial metrics  

2. **Feature Preprocessing**  
   - Select key numerical features (**Price, Market Cap, Volume, Percentage Change**)  
   - Apply **Min-Max Scaling** to normalize data  

3. **Anomaly Detection Models**  
   - **Isolation Forest**: Detects outliers based on how easily they can be isolated  
   - **DBSCAN**: Clusters normal data points and labels low-density points as anomalies  

4. **Results & Analysis**  
   - Compare **anomalies detected** by both models  
   - Export the results to `crypto_anomalies.csv`  

---

##  Tools & Technologies  
- **Programming Language:** Python  
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn  
- **Anomaly Detection Models:**  
  - `IsolationForest` (from Scikit-learn)  
  - `DBSCAN` (from Scikit-learn)  

---

## Exploratory Data Analysis (EDA)  
### Data Visualization  
- Price & Market Cap Distribution  
- Trading volume trends over time  
- Heatmaps for feature correlation  

### Sample Distribution Plot  
![image](https://github.com/user-attachments/assets/8e6bea02-5cde-4958-9826-771e62ba2c3c)
![Screenshot 2025-02-24 232537](https://github.com/user-attachments/assets/25497cbf-b0a5-492d-b701-341e6a7a9d76)

---

### 1Install Dependencies  
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
