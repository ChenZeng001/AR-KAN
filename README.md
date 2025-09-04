# AR-KAN: Autoregressive-Weight-Enhanced Kolmogorov–Arnold Network for Time Series Forecasting

This repository contains the official implementation of the paper:

**[AR-KAN: Autoregressive-Weight-Enhanced Kolmogorov–Arnold Network for Time Series Forecasting](https://arxiv.org/abs/2509.02967)**

Based on the Universal Myopic Mapping Theorem, we use the Kolmogorov-Arnold Network (KAN) as the static nonlinear part and design the memory structure using a pre-trained AR model. In our experimental results, AR-KAN achieved the best performance on 72% of the real-world datasets.

---

## 🛠️ Environment Setup

We recommend using **Python 3.9** with the following required packages. You can install them with:

```bash
pip install -r requirements.txt
```

In addition, please manually install the appropriate version of **PyTorch** by visiting the official website:

👉 https://pytorch.org/get-started/locally/

---

## 🚀 Code Usage

The purpose of each `.ipynb` file is as follows:

- **`datasets_save.ipynb`**  
  Downloads selected time series from the Rdatasets collection, performs normalization, and saves the processed data into the `datasets/` folder.

- **`AR_predict_functions.ipynb`**  
  Trains AR-MLP or AR-KAN models on almost-periodic functions.

- **`AR_predict_dataset.ipynb`**  
  Trains AR-MLP or AR-KAN models on real-world time series downloaded by **`datasets_save.ipynb`**.

