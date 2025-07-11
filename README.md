# Oxford Risk Behavioural Data Science Intern Application
## Saachi Sabnis



# Explanatory Data Analysis


Traditional financial models assume rational behaviour - yet real-world investors are heavily affected by their psychological traits biases - such as risk and loss aversion, impulsivity, or overconfidence - that shape their asset allocation strategies. Many financially sound decisions are emotionally uncomfortable like investing during market dips or resisting impulsive spending. 

This analysis aims to explore how individuals with varying personality traits - including risk tolerance, confidence, composure, impulsivity, and impact desire - allocate their financial assets. By examining this relationship, we seek to understand how emotional comfort, or the lack of it, shapes investor choices.

Why this matters:

--> People often avoid markets not because of lack of money, but due to emotional illiquidity—an inability to take action in moments of perceived loss.

--> Investors tend to offload rising assets and hold onto losing ones, driven by a desire to avoid realizing losses, rather than rational portfolio logic.


This EDA explores how behavioral tendencies manifest in asset allocations - such as whether impulsive individuals prefer speculative assets like crypto, or if confident individuals invest more overall. It also considers the role of personalization in bridging the “behavior gap”: the difference between what’s logically optimal and what people actually do.



# Histograms

These histograms show the distribution of the five key personality traits across the inidividuals in the dataset. Notably, majority of these follow a normal distribution, suggesting a natural variation around the average. This indicates that most people exhibit average levels of confidence, risk tolerance and composure with a few individuals on the extremes. The greater variation in impulsivity suggests that people differ significantly in their impulsivity levels and there is no "average" impulsive individual. Similarly, since impact_desire is uniformally distributed, this indicates that people vary widely in how strongly they are motivated to make a difference or influence outcomes. These results can strongly inform how people make financial decisions (for e.g. through investing in high risk-high reward funds, how diversified their portfolio may be, etc)


## How do personality traits correlate with each other and asset value?

The correlation matrix shows that confidence, risk tolerance, and composure are interrelated traits. People who are more confident tend to be more risk-seeking and also tend to be more composed. However, none of the personality traits showed a strong correlation with total asset value. This implies that while psychological traits may influence decision - making style, they do not independently explain how much individuals invest - this means that it is still important to consider social, economic and demographic context for e.g. what life stage they are in, their earnings, their cultural background, etc.



# How do asset allocation preferences vary by risk tolerance levels?

This chart shows patterns in how asset preferences vary by risk tolerance level. Individuals with high risk tolerance allocate a majority of their assets to crypto, indicating strong risk appetite and a tendency for high-volatility investments. In contrast, medium risk individuals exhibit a more balanced portfolio across asset classes, consistent with diversification strategies. Additionally, while low and medium risk customers still include a safe investment in the form of bonds, the high risk investors do not include bonds in their portfolio. This Interestingly, even low risk individuals show a significant share of crypto holdings, suggesting either some inconsistency or an acceptance of small, high-risk exposures within otherwise conservative portfolios.   highlights that while risk tolerance influences asset allocation, it does not fully dictate it - suggesting a role for emotional, contextual, or cognitive biases in investment choices.





# Next Steps and Recommendations



### 1. Collect Additional Contextual and Behavioural Data

To better understand user personas and improve predictive modeling, expand the dataset with:

- **Demographic data**:  
  Age, income, employment status, education level  
  ➤ Helps estimate financial capacity, life stage, and investment literacy

- **Historical investment behavior**:  
  Types of past investments, holding periods, timing of entry/exit, past outcomes  
  ➤ Useful for building behavioural profiles and validating consistency over time

- **Outcome data**:  
  Returns, losses, volatility exposure  
  ➤ Enables performance-adjusted analysis (e.g. comparing confidence with actual success)

---

### 2. Apply Machine Learning Models for Prediction

#### Feature Selection & Insight  
Using mdoels like Random Forest or XGBoost to identify which personality traits or demographic factors are most predictive of outcomes (e.g. asset mix, investment frequency) and detect non-linear interactions between traits.


---

###  Potential Modelling Ideas

1. **Classification Models**  
   Predict whether users are conservative, balanced, or aggressive investors based on traits and context.

2. **Clustering Behavioural Personas**  
   Use unsupervised techniques like **K-Means** or **DBSCAN** to reveal natural user types (e.g., high impulsivity + low composure).

3. **Predicting the Likelihood of Emotionally Driven Behaviour**  
   Estimate the likelihood of emotionally driven behavior such as **panic selling** or **overreacting to losses**.
