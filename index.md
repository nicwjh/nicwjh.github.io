---
layout: homepage
noindex: true
---

## About Me

I am a graduate student at MIT broadly interested in computational and statistical methods for problems in economics and finance. My work spans optimization, statistical learning, causal inference, and forecasting, with applications to financial markets, policy evaluation, and economic decision-making.

Previously, I graduated from UNC Chapel Hill with a B.S. in Computer Science, B.S. in Economics, and minor in Statistics and Analytics.   

## Research Interests

- **Primary:** computational methods, statistical inference, optimization, and machine learning, with applications to financial and economic systems.

## Research

<!--
### In progress
-->

#### Double Descent in Financial Time Series

*Research project for 6.7960 Deep Learning, MIT. Course supervised by Dr. Sara Beery, Dr. Kaiming He, Dr. Omar Khattab (MIT).*

*Blog post:* [Double Descent in Financial Time Series](http://nicwong.com/double-descent-in-financial-time-series/)      

*Paper:* [Double Descent](https://nicwong.com/assets/files/DDiFTS_v1.pdf)

_Abstract:_  
Modern deep learning models often exhibit double descent, where test error worsens near the interpolation threshold but improves again in the overparameterized regime. While this phenomenon is well documented in high-signal domains such as vision and language, its relevance for financial time series, which are noisy and non-stationary, remains unclear. We study whether the benefits of overparameterization extend to low signal-to-noise environments.

The results show that double descent requires sufficiently strong and stable signal: as noise increases, the interpolation peak attenuates and eventually disappears, and simpler models dominate. In equity return prediction, test error curves are nearly flat across four orders of magnitude in model size, and no configuration outperforms a naive mean benchmark. These findings provide empirical evidence that modern “bigger is better” intuitions do not generalize to low-signal, non-stationary settings and that classical model selection remains essential in financial forecasting.


#### Portfolio Optimization

*Research project conducted at Harvard University, supervised by Dr. Soroush Saghafian (HKS).*         
<!--
*Code:* [GitHub – Portfolio Optimization](https://github.com/nicwjh/Portfolio-Optimization)
-->

*Paper:*[Portfolio Optimization](https://nicwong.com/assets/files/Portfolio_Optimization.pdf)

_Abstract:_  
We propose a machine learning–based portfolio construction framework that integrates ensemble return forecasting with sparsified mean–variance optimization. I combine four supervised forecasting methods—Weighted Moving Average (WMA), Principal Components Regression (PCR), Random Forests, and Gated Recurrent Unit (GRU) networks—to predict returns for NASDAQ-100 constituents. Predicted returns are then aggregated and fed into a Markowitz mean–variance optimization problem with an L1 penalty to induce sparse, interpretable portfolio weights.

Using daily equity data from November 2023 to November 2024, the optimized portfolio achieves substantially higher risk-adjusted performance than a market-capitalization-weighted NASDAQ-100 benchmark. While the benchmark delivers higher absolute returns during the sample period, the optimized portfolio exhibits significantly lower volatility and a Sharpe ratio of 2.23, representing roughly a 40% improvement over the benchmark. Forecasting results highlight the robustness of simple and non-parametric methods while ensembling mitigates model-specific bias.

The results illustrate how modern machine learning forecasts can be systematically integrated with classical portfolio theory to improve risk-adjusted returns, and how sparsity constraints help address overfitting, high dimensionality, and investor preferences for concentrated portfolios.

#### Large Language Models in Equity Research
With Y. Pan, X. Fang, and C. Saad

*Joint Research Project (PanAgora Asset Management, MIT Sloan Finance Lab). Supervised by Dr. Gita Rao and Dr. Bhushan Vartak (MIT).*

*Poster:* [LLMs in Equity Research](https://nicwong.com/assets/files/panagora_poster.pdf)

*Paper:* [LLMs in Equity Research](https://nicwong.com/assets/files/llms_equity_research.pdf)

_Abstract:_
We study whether large language models can extract useful information from financial statements for fundamental equity research. Using anonymized balance sheet and income statement data, we prompt LLMs to perform trend analysis, ratio analysis, and to predict the direction and magnitude of future earnings changes. We compare LLM-based predictions to human analyst forecasts and to standard ML (XGBoost).

While LLMs alone do not consistently outperform simple benchmarks in predicting earnings changes, their outputs contain complementary information. When LLM-generated signals and embeddings are combined with financial statement data in downstream machine learning models, predictive performance improves and leads to economically meaningful portfolio results. Long-only portfolios formed using LLM-enhanced signals achieve higher alpha and information ratios than portfolios based on traditional factors or analyst forecasts. The findings suggest that LLMs add value by providing economic context and structure to raw accounting data, improving generalization in out-of-sample equity prediction tasks.

#### Macroeconomic Forecasting of Non-Farm Payrolls

*Macro Research Intern, Verition Fund Management. Supervised by Nisarg Kamdar (Portfolio Manager, Fixed Income & Macro).*

<!--
*Code:* [GitHub – NFP Forecasting](https://github.com/nicwjh/nfp-forecasting)
-->

_Abstract:_  
We develop a fully out-of-sample forecasting framework for U.S. Non-Farm Payroll (NFP) Total Change, a high-impact macroeconomic release central to rates and macro trading. Using historical economist forecasts, I construct ensemble point forecasts and calibrated predictive distributions designed for trading and risk management rather than purely statistical accuracy.

The approach combines adaptive forecast-combination methods—including inverse-error weighting, exponentially weighted schemes, multiplicative weights updates, and Bayesian model averaging—with distributional modeling using Student-t, Gaussian mixture, and t-GARCH specifications. Empirically, ensemble forecasts improve directional accuracy relative to consensus, while uncertainty-aware models deliver well-calibrated prediction intervals across business-cycle regimes. The results highlight the importance of robust aggregation and explicit uncertainty quantification in non-stationary macroeconomic environments and provide a generalizable framework for forecasting and risk management around scheduled macro events.


#### Regulatory Response to the SVB Collapse: A Natural Language Processing Analysis
With [P. Clark](https://priscillaoclark.github.io/)

*Research Project for 15.S08 Applied Natural Language Processing, MIT. Supervised by Dr. Mike Chen and Dr. Andrew Zachary (MIT).*

<!--
*Code:* [GitHub – SVB Regulatory Impact NLP](https://github.com/priscillaoclark/svb-regulatory-impact-nlp)
-->

_Abstract:_  
This project studies how U.S. banking regulatory priorities shifted following the 2023 collapse of Silicon Valley Bank (SVB). We test the hypothesis that regulatory focus intensified around liquidity, capital adequacy, and the oversight of small and mid-sized banks in the aftermath of the crisis. Using regulatory documents from Regulations.gov, we analyze proposed and finalized rules issued by major financial regulators in the 18 months before and after the collapse.

We apply three complementary NLP approaches: a naive keyword-based baseline, TF–IDF weighting, and BERTopic topic modeling. Across all methods, we find consistent evidence of a post-SVB pivot toward liquidity management, capital requirements, valuation practices, and systemic risk oversight. Topic models reveal a shift from broader regulatory themes pre-SVB to more concentrated attention on risk management, resolution frameworks, and financial stability post-SVB. The results provide empirical evidence that major financial crises are followed by measurable and systematic changes in regulatory discourse, and demonstrate how modern NLP tools can be used to study policy responses to financial instability at scale.

#### Evaluating CFTC COT Data as a Predictor of Treasury-Futures Returns
*Research project for 15.437 Options & Futures, MIT.*


*Paper:* [Evaluating CFTC COT Data as a Predictor of Treasury-Futures Returns](https://nicwong.com/assets/files/Options_Extra_Credit.pdf)

We test whether weekly Managed-Money positions from CFTC Commitments of Traders reports predict one- to two-week returns on 2-year and 10-year U.S. Treasury futures over 2011 to 2025. Using publication-lagged signals, HAC-corrected predictive regressions, expanding-window out-of-sample evaluation, and 
a sign-based trading backtest, we find no statistical or economic forecasting power. Out-of-sample R-squared values are negative across all specifications and Sharpe ratios are indistinguishable from zero, consistent with the view that public position disclosures are rapidly incorporated into prices in
 liquid Treasury markets.


#### Artificial Intelligence for Financial Analysis
With C. Shan, A. Wakrim, M. Walcher, D. Xiang, I. Xiao, J. Xu, and R. Yamahara.


*Joint Research Project (T. Rowe Price, MIT Sloan Proseminar in Capital Markets). Supervised by Mark Kritzman (MIT) and Sébastien Page (T. Rowe Price).*  
*Deck:* [Artificial Intelligence for Financial Analysis](http://nicwong.com/assets/files/T-Rowe-Final-Deck.pdf)

_Abstract:_  
We study whether modern generative AI models can perform analyst-level equity research. Using Microsoft and Chipotle as representative case studies (diversified, multi-segment vs pure-play, single business), we design a three-layer evaluation framework that progressively increases data quality and prompting sophistication, and compare AI-generated reports to professional analyst outputs.

Results show that richer inputs and structured prompting substantially improve report quality, including financial summaries, valuation, and investment recommendations. However, AI outputs still lack analytical depth, consistency, and contextual judgment relative to human analysts, especially for complex, diversified firms. The findings suggest that generative AI is best used as an analyst productivity tool rather than a replacement, augmenting routine financial analysis while human expertise remains critical for nuanced investment decisions.


#### Other Projects

#### Predicting Stock Price Movements from Social Media Sentiment
With J. Bourseau, C. Casper, and L. Valette

*Research project for 15.776 Intensive Hands-on Deep Learning, MIT.*

We frame next-day stock price direction as a binary classification task using aggregated daily tweet data for 11 publicly traded companies. We compare TF-IDF baselines (Logistic Regression, MLP) against BERT with a trained MLP head. All models perform near chance (AUC-ROC ≈ 0.50), with BERT underperforming simpler baselines. Results highlight the low signal-to-noise ratio in social media text for short-term prediction and the failure of general-purpose language representations to transfer to financial forecasting without domain-specific adaptation.

#### Multi-Factor Growth Stock Selection
With C. Sun, H. Zhang, and M. Goyal

*Research project for 15.433 Financial Markets, MIT.*

We develop a quarterly sliding-window linear regression framework to predict forward 12-month returns for Russell 1000 Growth Index constituents using five growth-oriented factors. Top-decile portfolios constructed from predicted returns achieve a 71.4% hit ratio and 2.14% annualized excess return over the benchmark. A long-short extension improves performance to a 0.61 Sharpe ratio and 80% hit ratio. Debt-to-Equity and Price-to-Book are identified as the most consistently significant predictors.


#### Review Helpfulness Classification via LLM Fine-Tuning
With C. Arraya, L.H. Cham, I. Sparrow, L. Yang, and T. Zhang

*Research project for COMP 488 Data Science in Business, UNC.*       

We fine-tune RoBERTa-base to classify Airbnb reviews into three helpfulness tiers (A/B/C) based on specificity, decision-making advice, and reviewer expertise. Training labels are generated synthetically using GPT-4 Turbo on 4,500 scraped reviews, while the test set of 500 reviews is manually labeled by majority vote. The fine-tuned classifier achieves 64.6% accuracy and 0.59 F1 on the human-labeled test set, with the strongest precision on least-helpful reviews and the weakest recall on most-helpful reviews.

<!--	#### Airbnb Price Prediction
*Research project for ECON 573 Machine Learning/Econometrics, UNC Chapel Hill.*

We compare four supervised regression methods for predicting Airbnb listing prices across major U.S. cities: forward selection, LASSO, polynomial regression, and gradient boosting. Boosting achieves the lowest test RMSE (85.11), outperforming linear methods by approximately 15%. A robust feature selection process across all models identifies maximum occupancy indicators (bathrooms, accommodates) and geographic features (latitude, longitude, city) as the most significant predictors of listing price.

#### Diabetes Classification with Limited Feature Sets
With H. Brinklert

*Research project for COMP 562 Honors Machine Learning, UNC Chapel Hill.*

We compare five classifiers (logistic regression, Naive Bayes, KNN, decision trees, SVM) for binary diabetes classification using both a full 21-feature set and a reduced 7-feature subset identified through LASSO, sequential selection, and domain knowledge. Models with fewer features achieve comparable performance to full-feature models across all classifiers. Naive Bayes and SVM perform best with limited inputs, while decision trees show signs of overfitting with the full feature set, achieving better results with fewer predictors. -->


## Other Links

- Sample research papers:
	- [(1) Double Descent in Financial Time Series](https://nicwong.com/assets/files/DDiFTS_v1.pdf) 
	- [(2) Portfolio Optimization](https://nicwong.com/assets/files/Portfolio_Optimization.pdf)
	- [(3) LLMs in Equity Research](https://nicwong.com/assets/files/llms_equity_research.pdf)
	- [(4) NFP Forecasting](https://nicwong.com/assets/files/nfp-forecasting.pdf)
	- [(5) SVB Collapse—NLP Analysis](https://nicwong.com/assets/files/NLP_SVBcollapse.pdf)
	- [(6) Artificial Intelligence for Financial Analysis](https://nicwong.com/assets/files/T-Rowe-Final-Report.pdf)
	- [(7) Evaluating CFTC COT Data as a Predictor of Treasury-Futures Returns](https://nicwong.com/assets/files/Options_Extra_Credit.pdf)
- Economics writing sample (DiD/RD causal identification study): [Effectiveness of a Managerial Training Program](https://nicwong.com/assets/files/Wong_Nicholas_Report.pdf)
<!--
- Other projects:
        · [(1) Multi-Factor Growth Stock Selection](https://nicwong.com/assets/files/AlphaGrowth__Identifying_Winning_Growth_Stocks.pdf)
	· [(2) Predicting Stock Price Movements from Social Media Sentiment](https://nicwong.com/assets/files/HODL_report.pdf)
        · [(3) Review Helpfulness Classification via LLM Fine-Tuning (Deck)](https://nicwong.com/assets/files/488_Final_Presentation.pdf)
        · [(4) Diabetes Classification with Limited Feature Sets](https://nicwong.com/assets/files/COMP562H_Nicholas_Hannes_Final_Report.pdf)
	· [(5) Airbnb Price Prediction](https://nicwong.com/assets/files/Nicholas_Wong_ECON573_FinalReport.pdf)  -->
- News: [Phi Beta Kappa Induction](https://uncnews.unc.edu/2023/04/06/219-students-inducted-into-phi-beta-kappa-at-unc-chapel-hill/)
