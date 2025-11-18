# Bitcoin 7-Day Price Forecaster (Temporal Fusion Transformer) 

**Live, auto-updating Bitcoin price forecaster** using Google & Uber's production-grade **Temporal Fusion Transformer** — the same model used at Google, Uber, Amazon, and top hedge funds.

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1JvHqFTY1D2jdeDwxlz0uDMYfJ9QdVC9w?usp=sharing)
[![Python](https://img.shields.io/badge/Python-3.10-blue)](https://python.org)
[![Darts](https://img.shields.io/badge/Darts-0.30-orange)](https://unit8co.github.io/darts/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

### Live Demo (click the badge above)
→ Opens a **real-time dashboard** that:
- Pulls the latest Bitcoin price from CoinGecko
- Generates a fresh 7-day forecast instantly
- Auto-refreshes every 10 minutes
- Loads the trained model from Google Drive in ~5 seconds (no retraining!)

### Key Features
- **Temporal Fusion Transformer** (state-of-the-art global forecasting model)
- Probabilistic forecasting with 80% confidence bands
- Live data pipeline (CoinGecko API)
- Model persistence in Google Drive – never train again
- Hourly Bitcoin data (1+ year history)
- Calendar features (hour, day-of-week, day-of-month) for strong seasonality capture
- Log-price transformation for stable training

### Performance (on validation set)
- 24-hour MAPE : ~2.7–3.5%
- 7-day MAPE   : ~5.5–7.0%
- MASE < 1.0 (beats naive seasonal baseline)

### Tech Stack
- Python + Darts (u8darts) + PyTorch
- Plotly for visualization
- Google Colab + Google Drive (persistent model storage)

### How to Run Locally or in Colab
1. Open the Colab badge above
2. Run all cells
3. Watch the live forecast update automatically

### Trained Model (saved in Google Drive – loads in 5 seconds)
Folder with full TFT checkpoint + scalers: [Click here to see model files](https://drive.google.com/file/d/1F14gqeDkUGkZGftFEwHPuIcfN0XkA_nM/view?usp=sharing))

