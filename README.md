# Variational Bayes for Limit Order Book Estimation

This repository contains the code, models, and results for the project **"Variational Bayes for Limit Order Book Estimation: A Probabilistic Approach to High-Frequency Trading"**. The project was developed as part of the AMS 522 course at Stony Brook University.

## 📌 Project Summary

We develop a **Variational Bayes (VB)** framework to estimate the latent fair price in high-frequency limit order book (LOB) data, comparing it to the gold-standard **Markov Chain Monte Carlo (MCMC)** inference using the No-U-Turn Sampler (NUTS). The latent price shocks are modeled as deviations from the mid-price and used to generate trading signals.

## 🔧 Features

* Latent-variable model of LOB ask and bid prices using transformed exponential priors.
* Scalable VB inference with stochastic optimization.
* MCMC sampling via NUTS for benchmarking.
* Signal generation and backtesting on real Binance BTC–USDT data.

## 🧪 Results

* VB is \~4× faster than MCMC with competitive performance.
* VB achieves higher Sharpe ratio and hit rate in backtests despite overestimating uncertainty.
* Visual and quantitative analysis of posterior divergence (KL divergence, density plots).


## 📄 Report

For a detailed explanation, see [`Bayes_report_final.pdf`](./Bayes_report_final.pdf).

## 🧑‍💻 Author

Matvei Lukianov
Quantitative Finance, Stony Brook University
[matvei.lukianov@stonybrook.edu](mailto:matvei.lukianov@stonybrook.edu)
