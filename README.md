# SharpeEdge – Code

Companion code for the **SharpeEdge** YouTube channel, which covers algorithmic trading and quantitative research in Python.

📺 **YouTube:** [SharpeEdge](https://www.youtube.com/@SharpeEdge)

Each video has its own folder with the Jupyter notebook shown on screen, so you can follow along, run it yourself and experiment with it.

## How it works

- Every folder is **self-contained and independent** from the others: pick the video you are interested in and open its notebook.
- Each notebook lists its dependencies in the first cell (`pip install ...`) and uses only relative paths, so it runs from scratch on any machine.
- Market data comes from [`yfinance`](https://github.com/ranaroussi/yfinance), from small datasets included in the video folder, or from public Kaggle datasets downloaded automatically by the notebook.
- Charts are interactive [Plotly](https://plotly.com/python/) figures.

## Getting started

```bash
git clone https://github.com/pietrobelli26/sharpe_edge_code.git
cd sharpe_edge_code

python -m venv .env
source .env/bin/activate        # Windows: .env\Scripts\activate

pip install jupyter             # then the packages listed in the notebook's first cell
jupyter lab
```

Open the notebook of the video you want and run it top to bottom.

## Repository structure

| Folder | Topic |
| --- | --- |
| [`logistic_regression/`](logistic_regression/) | Logistic regression for trading signals |
| [`signal_filter_svm/`](signal_filter_svm/) | Meta-labeling: filtering trading signals with an SVM (Nasdaq 100 data downloaded from Kaggle) |
| [`prop_firm_monte_carlo/`](prop_firm_monte_carlo/) | Monte Carlo simulation of prop firm challenges |
| [`live_monitoring/`](live_monitoring/) | Monitoring a live strategy |
| [`kalman_trend_filter/`](kalman_trend_filter/) | Trend filtering with a Kalman filter |
| [`portfolio_management/`](portfolio_management/) | Portfolio management |

Each folder contains only the video's notebook and, where needed, its small datasets.

## Disclaimer

This repository is for **educational purposes only** and is not financial advice. The backtests in the notebooks are demonstrations of a technique, not validations of a tradable strategy. Past performance does not guarantee future results; trading involves risk of loss.

## License

Released under the [MIT License](LICENSE).
