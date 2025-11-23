
# Predicting Price Moves with News Sentiment

**10 Academy Artificial Intelligence Mastery - Week 1 Challenge**

## 📖 Overview
This project focuses on the detailed analysis of a large corpus of financial news data to discover correlations between news sentiment and stock market movements. The goal is to refine skills in Data Engineering (DE), Financial Analytics (FA), and Machine Learning Engineering (MLE) by simulating a real-world task for **Nova Financial Solutions**.

## 🎯 Business Objective
**Nova Financial Solutions** aims to enhance its predictive analytics capabilities to significantly boost financial forecasting accuracy and operational efficiency. 

As a Data Analyst, the primary task is to:
1.  **Sentiment Analysis:** Quantify the tone (positive, negative, neutral) of financial news headlines.
2.  **Correlation Analysis:** Establish statistical correlations between derived sentiment scores and corresponding stock price movements (daily returns).
3.  **Investment Strategy:** Provide actionable insights and strategies based on the relationship between news sentiment and stock fluctuations.

## 📂 Project Structure

```text
├── .vscode/
│   └── settings.json
├── .github/
│   └── workflows
│       └── unittests.yml
├── .gitignore
├── requirements.txt
├── README.md
├── src/
│   ├── __init__.py
├── notebooks/
│   ├── __init__.py
│   ├── 1_eda_financial_news.ipynb
│   ├── 2_quantitative_analysis.ipynb
│   └── 3_correlation_analysis.ipynb
├── tests/
│   ├── __init__.py
└── scripts/
    ├── __init__.py
    └── README.md
````

## 🛠️ Installation & Setup

### Prerequisites

  * Python 3.8+
  * Git

### Step-by-Step Setup

1.  **Clone the Repository**

    ```bash
    git clone https://github.com/Yeabfikre/financial-news-sentiment.git
    cd financial-news-sentiment
    ```

2.  **Create a Virtual Environment**

    ```bash
    # Windows
    python -m venv venv
    source venv/Scripts/activate 

    # macOS/Linux
    python3 -m venv venv
    source venv/bin/activate
    ```

3.  **Install Dependencies**
    *Note: This project requires `TA-Lib`, which may need to be installed as a binary before running pip.*

    ```bash
    pip install -r requirements.txt
    ```

## 📊 Data Overview

The project uses the **FNSPID (Financial News and Stock Price Integration Dataset)**.

  * **headline:** Article release headline.
  * **url:** Direct link to the article.
  * **publisher:** Author/creator.
  * **date:** Publication date and time (UTC-4).
  * **stock:** Stock ticker symbol (e.g., AAPL).

* **Note:** Raw data files are not included in this repository to ensure compliance with data size limits. Please download the dataset locally and place it in a `data/` folder (ignored by git).*

## 🚀 Key Tasks Implemented

### Task 1: Exploratory Data Analysis (EDA)

  * **Descriptive Statistics:** Analyzed headline lengths and article counts per publisher.
  * **Text Analysis:** Performed topic modeling/keyword extraction to identify significant financial events.
  * **Time Series:** Analyzed publication frequency spikes related to market events and specific publishing times.
  * **Publisher Analysis:** Identified top publishers and unique domains .

### Task 2: Quantitative Analysis

  * **Indicators:** Calculated technical indicators using `TA-Lib` and `PyNance`:
      * **Moving Averages (SMA/EMA)**
      * **RSI (Relative Strength Index)**
      * **MACD (Moving Average Convergence Divergence)**.
  * **Visualization:** Plotted stock prices alongside indicators to visualize market trends.

### Task 3: Correlation Analysis

  * **Date Alignment:** Normalized timestamps to align news frequency with daily stock trading days.
  * **Sentiment Scoring:** Used NLP (TextBlob) to assign polarity scores to headlines.
  * **Correlation:** Calculated the **Pearson correlation coefficient** between average daily sentiment scores and daily stock returns.

## 📈 Results & Insights

  * *The correlation between news sentiment and Apple's stock price is essentially zero (0.0116), indicating that daily sentiment does not have a meaningful immediate impact on daily price levels.*

## 🤝 Contributing

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

## 👤 Author

**Yeabsira Fikre**

  * 10 Academy - AI Mastery Trainee
  * https://www.linkedin.com/in/yeabsira-fikre

<!-- end list -->

