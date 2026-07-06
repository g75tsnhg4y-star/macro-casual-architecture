# Structural Causal Architecture & Live Dashboard

## 🚀 Access the Live Dashboard
**[Click here to launch the Quant Macro Dashboard](YOUR_SHINYAPPS_IO_URL_HERE)**

## Project Overview
This repository contains the architecture for a real-time macroeconomic causal inference engine. While the core research was conducted using **Constraint-Based Structure Learning** via the Hill-Climbing algorithm, the architecture has been evolved into a live production dashboard.

## Key Features (v3.2)
* **Global Macro Engine:** Now supports dynamic ticker input for any global asset, moving beyond the original Nifty Bank focus.
* **Continuous Allocation:** Implemented a continuous NLP sentiment scaling engine (replacing rigid buckets) to provide precision portfolio weights.
* **Spurious Correlation Removal:** All historical data is now processed via daily log-returns to strip time-series trends and reveal true structural edges.
* **Tail-Risk Awareness:** Utilizes Bayesian Network boot-strapping to confirm edge robustness in real-time.

## Tech Stack
* **Language:** R
* **Framework:** Shiny
* **Libraries:** `bnlearn` (Bayesian Learning), `quantmod` (Financial Data), `syuzhet` (NLP Sentiment), `rvest` (Web Scraping)
* **Deployment:** ShinyApps.io
