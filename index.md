---
layout: homepage
noindex: true
---

## About Me

I am a graduate student at MIT broadly interested in computational and statistical methods for problems in economics and finance. My work spans optimization, statistical learning, causal inference, and forecasting, with applications to financial markets, policy evaluation, and economic decision-making.

Previously, I graduated from UNC Chapel Hill with a B.S. in Computer Science, B.S. in Economics, and minor in Statistics and Analytics.   

## Research Interests

I'm broadly interested in computational methods, statistical inference, optimization, and machine learning, with applications to financial and economic systems.

- **Primary:** asset pricing, market microstructure, machine learning in finance
- **Other interests:**  household finance, macroeconomics

## Research


#### Double Descent in Financial Time Series

*Research project for 6.7960 Deep Learning, MIT. Course supervised by Dr. Sara Beery, Dr. Kaiming He, Dr. Omar Khattab (MIT).*

*Blog post:* [Double Descent in Financial Time Series](http://nicwong.com/double-descent-in-financial-time-series/)      

*Paper:* [Double Descent](https://nicwong.com/assets/files/DDiFTS_v1.pdf)

_Abstract:_  
Modern deep learning models often exhibit double descent, where test error worsens near the interpolation threshold but improves again with overparameterization. We examine whether this behavior extends to financial time series, which are noisy and non-stationary. The interpolation peak attenuates and eventually disappears as noise rises, and in equity return prediction test error is nearly flat across four orders of magnitude in model size, with no configuration beating a naive mean benchmark. The results suggest that "bigger is better" intuitions from vision and language do not generalize to low-signal settings, and that classical model selection remains essential in financial forecasting.


#### Large Language Models in Equity Research
With Y. Pan, X. Fang, and C. Saad

*Joint Research Project (PanAgora Asset Management, MIT Sloan Finance Lab). Supervised by Dr. Gita Rao and Dr. Bhushan Vartak (MIT).*

*Poster:* [LLMs in Equity Research](https://nicwong.com/assets/files/panagora_poster.pdf)

*Paper:* [LLMs in Equity Research](https://nicwong.com/assets/files/llms_equity_research.pdf)

_Abstract:_
We test whether large language models can extract useful information from financial statements for fundamental equity research. On their own, LLMs do not consistently outperform simple benchmarks at predicting earnings changes. However, combining LLM-generated signals and embeddings with financial statement data in downstream ML models improves predictive performance, and long-only portfolios formed from these signals achieve higher alpha and information ratios than portfolios based on traditional factors or analyst forecasts. LLMs appear to add value by providing economic context and structure to raw accounting data, improving out-of-sample generalization.



#### Portfolio Optimization

*Research project conducted at Harvard University, supervised by Dr. Soroush Saghafian (HKS).*

*Paper:*[Portfolio Optimization](https://nicwong.com/assets/files/Portfolio_Optimization.pdf)

_Abstract:_
We propose a portfolio construction framework that combines ensemble return forecasts with L1-penalized mean-variance optimization. Four supervised methods (WMA, PCR, Random Forests, GRU) forecast returns for NASDAQ-100 constituents, and predictions feed into a sparsified Markowitz problem. On daily data from November 2023 to November 2024, the optimized portfolio achieves a Sharpe ratio of 2.23, roughly a 40% improvement over the market-cap-weighted benchmark, with substantially lower volatility. The results illustrate how machine learning forecasts can be integrated with classical portfolio theory, and how sparsity constraints help address overfitting, high dimensionality, and investor preferences for concentrated portfolios.


#### Macroeconomic Forecasting of Non-Farm Payrolls

*Macro Research Intern, Verition Fund Management. Supervised by Nisarg Kamdar (Portfolio Manager, Fixed Income & Macro).*

_Abstract:_
We develop a fully out-of-sample forecasting framework for U.S. Non-Farm Payroll Total Change, designed for trading and risk management rather than statistical accuracy alone. The approach combines adaptive forecast-combination methods (inverse-error weighting, exponentially weighted schemes, multiplicative weights updates, and Bayesian model averaging) with distributional modeling via Student-t, Gaussian mixture, and t-GARCH specifications. Ensemble forecasts improve directional accuracy relative to consensus, and uncertainty-aware models deliver well-calibrated prediction intervals across business-cycle regimes. The results highlight the value of robust aggregation and explicit uncertainty quantification around scheduled macro events.


#### Regulatory Response to the SVB Collapse: A Natural Language Processing Analysis
With [P. Clark](https://priscillaoclark.github.io/)

*Research Project for 15.S08 Applied Natural Language Processing, MIT. Supervised by Dr. Mike Chen and Dr. Andrew Zachary (MIT).*


_Abstract:_  
We study how U.S. banking regulatory priorities shifted following the 2023 collapse of Silicon Valley Bank. Using regulatory documents from Regulations.gov in the 18 months before and after the collapse, we apply three complementary NLP methods: a keyword baseline, TF-IDF weighting, and BERTopic topic modeling. All three show consistent evidence of a post-SVB pivot toward liquidity management, capital requirements, and systemic risk oversight, with topic models revealing a shift from broad regulatory themes to concentrated attention on risk management and financial stability. The work provides empirical evidence that major financial crises are followed by measurable changes in regulatory discourse.


#### Artificial Intelligence for Financial Analysis
With C. Shan, A. Wakrim, M. Walcher, D. Xiang, I. Xiao, J. Xu, and R. Yamahara.


*Joint Research Project (T. Rowe Price, MIT Sloan Proseminar in Capital Markets). Supervised by Mark Kritzman (MIT) and Sébastien Page (T. Rowe Price).*  

_Abstract:_  
We evaluate whether generative AI can perform analyst-level equity research, using Microsoft and Chipotle as representative case studies for diversified and pure-play businesses. A three-layer evaluation framework progressively increases data quality and prompting sophistication, and compares AI-generated reports to professional analyst outputs. Richer inputs and structured prompting substantially improve financial summaries, valuation, and recommendations, but AI outputs still lack the analytical depth and contextual judgment of human analysts, particularly for complex firms. Generative AI is best positioned as an analyst productivity tool rather than a replacement.


## Other Links

- Sample research papers:
        - [(1) Double Descent in Financial Time Series](https://nicwong.com/assets/files/DDiFTS_v1.pdf) 
        - [(2) LLMs in Equity Research](https://nicwong.com/assets/files/llms_equity_research.pdf)
        - [(3) Portfolio Optimization](https://nicwong.com/assets/files/Portfolio_Optimization.pdf)
        - [(4) NFP Forecasting](https://nicwong.com/assets/files/nfp-forecasting.pdf)
- Economics writing sample (DiD/RD causal identification study): [Effectiveness of a Managerial Training Program](https://nicwong.com/assets/files/Wong_Nicholas_Report.pdf)
- News: [Phi Beta Kappa Induction](https://uncnews.unc.edu/2023/04/06/219-students-inducted-into-phi-beta-kappa-at-unc-chapel-hill/)
