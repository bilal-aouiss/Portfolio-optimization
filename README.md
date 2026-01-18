# 📈 Clustering + LSTM Expected Returns + Portfolio Optimization (Markowitz) — Dashboard Streamlit

Ce projet construit une stratégie de trading quantitative sur l’univers **S&P 500** :

1. **Collecte des données** (tickers S&P500 depuis Wikipedia + prix OHLCV depuis Yahoo Finance)
2. **Feature engineering** (GK volatility, dollar volume, RSI, ATR…)
3. **Resample mensuel** + rendements multi-horizons
4. **Facteurs Fama-French** + **betas glissants** (Rolling OLS)
5. **Clustering mensuel (KMeans)** avec standardisation intra-mois
6. **Interprétation des clusters** (rôles : *Gagnants dynamiques*, *Stables de qualité*, etc.)
7. **Sélection d’un univers investissable** (top actions winners/stables)
8. **Modèle LSTM** pour prédire le **return_1m du mois suivant**
9. **Optimisation de portefeuille** (Efficient Frontier / Max Sharpe) avec contraintes (poids max, split winners/stables)
10. **Backtest** vs baseline equal-weight + comparaison à **SPY**
11. **Export** des artefacts pour le dashboard Streamlit

---

## ✅ Structure recommandée

