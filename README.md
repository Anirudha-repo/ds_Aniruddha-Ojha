### Trader Behavior and Market Sentiment Analysis

#### Overview

This project analyzes the relationship between trader performance on the Hyperliquid platform and the daily Bitcoin Fear & Greed Index. The goal is to uncover hidden patterns, correlations, and actionable insights that can drive smarter trading strategies.

#### Project Structure

The project is organized into the following directory structure:

```
ds_<candidate_name>/
├── notebook_1.ipynb           # Main analysis notebook
├── csv_files/                 # Stores raw and processed data
│   ├── fear_greed_index.csv
│   ├── historical_data.csv
│   └── merged_data.csv        # Processed data
│   └── ranked_traders_full.csv # Ranked traders list
├── outputs/                   # Stores all visual outputs
│   ├── sentiment_performance_bars.png
│   ├── correlation_heatmap.png
│   └── pnl_vs_sentiment_scatter.png
└── ds_report.pdf              # Final report with summarized insights
```

#### Project Components

1.  **Data Acquisition and Preparation**:

      * The analysis uses two primary datasets: Bitcoin Market Sentiment (`fear_greed_index.csv`) and Historical Trader Data (`historical_data.csv`).
      * Data cleaning and merging were performed to combine these datasets, associating each trade with the market sentiment on that day.

2.  **Analysis and Insights**:

      * **Sentiment Regimes**: Trader performance metrics (Average PnL, Win Rate) were calculated for each sentiment regime (`Fear`, `Greed`, `Neutral`).
      * **Contrarian Traders**: Identified traders who are most profitable during periods of market `Fear`, demonstrating contrarian strength.
      * **Correlation Analysis**: A correlation matrix and scatter plot were generated to visualize the relationship between the daily sentiment value and aggregated trading outcomes.
      * **Trader Leaderboards**: Ranked lists of traders were created based on various metrics, including `Total_PnL`, `Overall_Win_Rate`, and `Profit_Factor`, a key risk management metric.

3.  **Visualizations and Reporting**:

      * All key findings are visualized through charts and plots saved in the `outputs/` directory.
      * A final, detailed report (`ds_report.pdf`) summarizes the findings and provides strategic recommendations.
      * A Power BI dashboard was created to present the insights interactively.

#### Getting Started

1.  Clone this repository.
2.  Upload `fear_greed_index.csv` and `historical_data.csv` to your environment.
3.  Open `notebook_1.ipynb` in a Google Colab or Jupyter Notebook environment and run the cells to reproduce the analysis.
4.  Use the generated `merged_data.csv` and `ranked_traders_full.csv` to build a Power BI dashboard.
5.  Refer to `ds_report.pdf` for a detailed summary of the findings.
