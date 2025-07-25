# Objective 
Develop an enterprise‑grade predictive‑analytics solution that ingests raw customer transaction data, cleans and enriches it, and then forecasts each shopper’s likelihood of purchasing a newly launched Gold Membership offer. The goal is to optimize campaign targeting, reduce outreach costs, and improve conversion rates during the year‑end promotional cycle.

# Tech Stack
* Programming Language: Python
* Libraries: pandas, numpy, scikit-learn, matplotlib, Seaborn, datetime, Scipy
* Tools: Google Collab, Excel, Github

# Overview
Processed 2,240 customer records covering spending behavior, purchase recency, channel interaction, demographics, and complaint history. Conducted exploratory data analysis (EDA) using Python (pandas, Seaborn, matplotlib), engineered 30+ features, handled class imbalance using SMOTE, and deployed a soft-voting ensemble model (Logistic Regression, KNN, SVC). Workflow executed in Google Colab with full version control on GitHub and visualization support in Excel.

Key steps:
* Converted birth year into customer age for interpretable segmentation. <br>
* Created new metrics like total spend, total purchases, and web visits. <br>
* Removed multicollinear and low-importance features via correlation analysis and VIF scores. <br>
* Scaled numeric data and one-hot encoded categorical features. <br>
* Balanced classes to handle only 15% positive response using oversampling techniques. <br>

# Insights
1. Recency drives response – customers who purchased within the past 35 days were significantly more likely to opt in, versus an average of 51 days for non-members.

2. Education level influence – customers with PhDs showed a higher conversion tendency, suggesting targeted education-based segmentation may enhance ROI.

3. High-spend offsets low activity – shoppers with a long inactivity period still converted when their average order value was high (≥ $50).

4. Online activity signals intent – frequent web visitors (≥ 4/month) were more inclined to purchase the membership.

5. Complaint behavior negligible – only 1% of customers had prior complaints, suggesting minimal impact from negative experiences

# Conclusions / Recommendations
1. Targeted outreach – deploy propensity scores into the calling strategy to focus only on the top 30% most likely responders, cutting down operational costs.

2. Tailored messaging – prioritize digital-first customers and recent shoppers with personalized messaging; integrate purchase value as a driver for upsell.

3. Bundle and upsell – promote Wine & Meat premium bundles to high-spend customers; test price anchoring with $999 vs $499 offers for perceived value.

4. Digital nudges – trigger reminder calls or push notifications post web visits, especially when paired with limited-time offers.

5. Sustain improvements – establish MLflow-based model monitoring for version control, schedule monthly retraining, and feed learnings into quarterly performance reviews to refine campaign strategies and budget allocations
