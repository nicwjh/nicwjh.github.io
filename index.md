---
layout: homepage
---

## About Me

I'm a graduate student at MIT where most of my work has been focused on the intersection between finance and applied ML. 

Previously, I graduated from UNC Chapel Hill with a B.S. in Computer Science and Economics.   

## Research Interests

- **Primary:** algorithmic economics, empirical finance, asset pricing, computational methods

## Research

<!--
### In progress
-->

#### Double Descent in Financial Time Series

*Research project for 6.7960 Deep Learning, MIT.*

*Blog post:* [Double Descent in Financial Time Series](http://nicwong.com/double-descent-in-financial-time-series/)

_Abstract:_  
Modern deep learning models often exhibit double descent, where test error worsens near the interpolation threshold but improves again in the overparameterized regime. While this phenomenon is well documented in high-signal domains such as vision and language, its relevance for financial time series, which are noisy and non-stationary, remains unclear. This project studies whether the benefits of overparameterization extend to low signal-to-noise environments.

The results show that double descent requires sufficiently strong and stable signal: as noise increases, the interpolation peak attenuates and eventually disappears, and simpler models dominate. In equity return prediction, test error curves are nearly flat across four orders of magnitude in model size, and no configuration outperforms a naive mean benchmark. These findings provide empirical evidence that modern “bigger is better” intuitions do not generalize to low-signal, non-stationary settings and that classical model selection remains essential in financial forecasting.


#### Portfolio Optimization

*Research project conducted at Harvard University, supervised by Dr. Soroush Saghafian*

*Code:* [GitHub – Portfolio Optimization](https://github.com/nicwjh/Portfolio-Optimization)

_Abstract:_  
This project develops a machine learning–based portfolio construction framework that integrates ensemble return forecasting with sparsified mean–variance optimization. I combine four supervised forecasting methods—Weighted Moving Average (WMA), Principal Components Regression (PCR), Random Forests, and Gated Recurrent Unit (GRU) networks—to predict returns for NASDAQ-100 constituents. Predicted returns are then aggregated and fed into a Markowitz mean–variance optimization problem with an L1 penalty to induce sparse, interpretable portfolio weights.

Using daily equity data from November 2023 to November 2024, the optimized portfolio achieves substantially higher risk-adjusted performance than a market-capitalization-weighted NASDAQ-100 benchmark. While the benchmark delivers higher absolute returns during the sample period, the optimized portfolio exhibits significantly lower volatility and a Sharpe ratio of 2.23, representing roughly a 40% improvement over the benchmark. Forecasting results highlight the robustness of simple and non-parametric methods while ensembling mitigates model-specific bias.

The results illustrate how modern machine learning forecasts can be systematically integrated with classical portfolio theory to improve risk-adjusted returns, and how sparsity constraints help address overfitting, high dimensionality, and investor preferences for concentrated portfolios.

#### Macroeconomic Forecasting of Non-Farm Payrolls

*Macro Research Intern, Verition Fund Management. Supervised by Nisarg Kamdar (Portfolio Manager, Fixed Income & Macro).*

*Code:* [GitHub – NFP Forecasting](https://github.com/nicwjh/nfp-forecasting)

_Abstract:_  
This project develops a fully out-of-sample forecasting framework for U.S. Non-Farm Payroll (NFP) Total Change, a high-impact macroeconomic release central to rates and macro trading. Using historical economist forecasts, I construct ensemble point forecasts and calibrated predictive distributions designed for trading and risk management rather than purely statistical accuracy.

The approach combines adaptive forecast-combination methods—including inverse-error weighting, exponentially weighted schemes, multiplicative weights updates, and Bayesian model averaging—with distributional modeling using Student-t, Gaussian mixture, and t-GARCH specifications. Empirically, ensemble forecasts improve directional accuracy relative to consensus, while uncertainty-aware models deliver well-calibrated prediction intervals across business-cycle regimes. The results highlight the importance of robust aggregation and explicit uncertainty quantification in non-stationary macroeconomic environments and provide a generalizable framework for forecasting and risk management around scheduled macro events.

#### Regulatory Response to the SVB Collapse: A Natural Language Processing Analysis

*Research Project for 15.S08 Applied Natural Language Processing, MIT. Supervised by Dr. Mike Chen and Dr. Andrew Zachary (MIT).*

*Code:* [GitHub – SVB Regulatory Impact NLP](https://github.com/priscillaoclark/svb-regulatory-impact-nlp)

_Abstract:_  
This project studies how U.S. banking regulatory priorities shifted following the 2023 collapse of Silicon Valley Bank (SVB). We test the hypothesis that regulatory focus intensified around liquidity, capital adequacy, and the oversight of small and mid-sized banks in the aftermath of the crisis. Using regulatory documents from Regulations.gov, we analyze proposed and finalized rules issued by major financial regulators in the 18 months before and after the collapse.

We apply three complementary NLP approaches: a naive keyword-based baseline, TF–IDF weighting, and BERTopic topic modeling. Across all methods, we find consistent evidence of a post-SVB pivot toward liquidity management, capital requirements, valuation practices, and systemic risk oversight. Topic models reveal a shift from broader regulatory themes pre-SVB to more concentrated attention on risk management, resolution frameworks, and financial stability post-SVB. The results provide empirical evidence that major financial crises are followed by measurable and systematic changes in regulatory discourse, and demonstrate how modern NLP tools can be used to study policy responses to financial instability at scale.
