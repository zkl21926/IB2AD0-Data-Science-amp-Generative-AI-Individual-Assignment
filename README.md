# AI-Enhanced Momentum Strategy: Mitigating Crash Risk

## 📌 Overview
This project addresses the "Momentum Crash" phenomenon in financial markets. By integrating **Unsupervised Learning (K-Means Clustering)**, the model autonomously detects high-risk market regimes and dynamically hedges the portfolio, significantly reducing drawdowns during crises like 2009 and 2020.

## 📂 Repository Content

### 1. Theoretical Background
* **`Original_Momentum_Strategy_Paper.pdf`**
    * My original research paper detailing the mechanics and risks of Cross-Sectional Momentum strategies.

### 2. Data Source
* **`10_Portfolios_Prior_12_2.csv`**
    * Monthly returns of 10 portfolios (from Kenneth French Library) used to construct the Winners-Minus-Losers (WML) factor.

### 3. Code & Analysis
* **`01_Momentum_Crash_Analysis (1).ipynb`** (The Problem)
    * Implements the traditional baseline strategy.
    * **Finding:** Identifies a catastrophic **-81% drawdown** during the 2009 reversal.
    
* **`02_AI_Risk_Control.ipynb`** (The AI Solution)
    * Implements K-Means Clustering to identify "Panic" vs. "Safe" volatility regimes.
    * **Result:** The AI agent successfully avoids the crash, protecting capital.

## 📊 Key Results (Empirical Evidence)

| Metric | Traditional Strategy | AI-Enhanced Strategy | Impact |
| :--- | :--- | :--- | :--- |
| **2009 Crisis Drawdown** | **-81.1%** | **-29.0%** | **Significant Risk Reduction** |
| **Strategy Logic** | Linear | Non-Linear (Regime Based) | Adaptive Risk Control |

## 🛠️ Tech Stack
* **Python**: Pandas, NumPy
* **AI/ML**: Scikit-learn (K-Means Clustering)
* **Visualization**: Matplotlib
