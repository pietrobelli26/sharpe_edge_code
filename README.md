# SharpeEdge – Code

Companion code for the **SharpeEdge** YouTube channel, which covers algorithmic trading and quantitative research in Python.

📺 **YouTube:** [SharpeEdge](https://www.youtube.com/@SharpeEdge)

Each video has its own folder with the Jupyter notebook shown on screen, so you can follow along, run it yourself and experiment with it.

## How it works

- Every folder is **self-contained and independent** from the others: pick the video you are interested in and open its notebook.
- Each notebook lists its dependencies in the first cell (`pip install ...`) and uses only relative paths, so it runs from scratch on any machine.
- Market data comes from [`yfinance`](https://github.com/ranaroussi/yfinance) or from public Kaggle datasets downloaded automatically by the notebook.

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

| Folder | Topic | Video |
| --- | --- | --- |
| [`logistic_regression/`](logistic_regression/) | Logistic regression for trading signals | [Watch](https://youtu.be/jh4OlQQUaMc) |
| [`signal_filter_svm/`](signal_filter_svm/) | Meta-labeling: filtering trading signals with a SVM | [Watch](https://youtu.be/1_0d1peItok) |
| [`prop_firm_monte_carlo/`](prop_firm_monte_carlo/) | Monte Carlo simulation of prop firm challenges | [Watch](https://youtu.be/DTVjwgob_E8) |
| [`live_monitoring/`](live_monitoring/) | Monitoring a live strategy (alpha decay) | [Watch](https://youtu.be/CWOhChDdnn4) |
| [`kalman_trend_filter/`](kalman_trend_filter/) | Trend filtering with a Kalman filter | [Watch](https://youtu.be/nhY9xfK540Q) |
| [`portfolio_management/`](portfolio_management/) | Portfolio management | [Watch](https://youtu.be/XDnnBQqvQlE) |
| [`market_regimes/`](market_regimes/) | Market regime classification | [Watch](https://youtu.be/dzGEf3QWmXU) |
| [`pairs_trading/`](pairs_trading/) | Pairs trading: cointegration, hedge ratio and backtest | [Watch](https://youtu.be/_yrv7kb_CRY) |

## Disclaimer

This repository is for **educational purposes only** and is not financial advice. The backtests in the notebooks are demonstrations of a technique, not validations of a tradable strategy. Past performance does not guarantee future results; trading involves risk of loss.

## License

Released under the [MIT License](LICENSE).
