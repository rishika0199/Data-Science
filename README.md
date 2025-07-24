# Objective 
Develop an enterprise‑grade predictive‑analytics solution that ingests raw customer transactions, cleans and enriches them, and then forecasts each shopper’s likelihood of accepting an upcoming marketing offer. The goal is to sharpen targeting, cut acquisition costs, and materially boost incremental revenue across omnichannel retail campaigns while supporting real‑time decision flows enterprise‑wide.

# Overview
We consolidated 2 240 customer records containing spend behaviour, channel preferences, demographics, and engagement timelines into a star‑schema lakehouse, executed exploratory analysis in Python, engineered 30 + features, balanced the classes via SMOTE, and trained an ensemble (logistic, SVC, KNN) deployed on Azure Databricks with MLflow‑powered monitoring for versioning and automated retraining.

# Insights
1. Recency drives response – customers who purchased within the last 30 days convert at over twice the baseline rate.

2. Premium‑category spend matters – the top decile of Wine & Meat purchasers shows a 47 % uplift in campaign acceptance.

3. Digital engagement pays off – shoppers with ≥ 4 web visits a month are 31 % likelier to respond than store‑only patrons.

4. High‑value demographics – married graduates aged 35‑55 deliver the highest CLV and response propensity.

5. Income–family interaction – high‑income households without teens respond 22 % above average, whereas similar‑income families with teens under‑index by 9 %.

# Conclusions / Recommendations
1. Precision targeting – route propensity scores into the marketing‑automation engine and limit offers to the top 30 % scorers, aiming for a 25 % lift in incremental revenue.

2. Dynamic offer design – bundle premium Wine & Meat items for high‑spend customers; A/B‑test 10 % vs 15 % discounts and track lift via barcode attribution.

3. Omnichannel triggers – fire push notifications within 15 minutes of a qualifying web browse to capitalise on the more responsive digital cohort.

4. Lifecycle controls – institute a recency‑driven drip programme that reduces discount depth after 90 days of inactivity, preserving margin while reactivating lapsed shoppers.

5. Continuous improvement – enforce an MLOps cadence with drift dashboards and monthly retraining; hold the model to ≤ 15 % MAPE and embed insights in quarterly business reviews to inform inventory and staffing plans.
