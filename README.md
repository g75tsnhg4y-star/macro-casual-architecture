# Structural Causal Architecture of Macroeconomics

## Objective
Standard regression models suffer from severe endogeneity and omitted variable bias when analyzing macroeconomic systems. This project utilizes constraint-based structure learning to discover the true causal topology between global macro proxies and the Nifty Bank Index.

## Methodology
Instead of relying on basic correlation, this pipeline utilizes a **Directed Acyclic Graph (DAG)** via the Hill-Climbing machine learning algorithm to strip away noise and reveal underlying structural edges. 

To ensure the discovered topology is not a statistical anomaly, the network structure is stress-tested using **non-parametric bootstrap resampling** (100 iterations) to confirm the strength and directionality of the edges.

## Actionable Takeaway
Using Gold (`GLD`) as a live market proxy for inflation expectations and the US 10-Year Treasury (`^TNX`) as a global yield benchmark, the causal architecture mathematically proves that Yields and Inflation are root drivers of bank equity valuations. 

Because the inflation proxy possesses a direct, causal edge to the Nifty Bank index, the implied portfolio strategy is to dynamically increase interest-rate hedges in the 72 hours preceding a projected hot CPI print, as the structural topology dictates downstream damage to bank valuations.

## Tech Stack & Data
* **Language:** R
* **Libraries:** `quantmod` (Financial Data API), `bnlearn` (Bayesian Network Learning), `knitr`
* **Data Sources:** Live API extraction via Yahoo Finance

---
*Note: A fully compiled PDF of the research report, including the generated DAG and bootstrap confidence tables, is available in this repository.*
