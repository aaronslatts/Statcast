# Statcast
IS445 StatCast Data Project
⚾ Modern MLB Performance: Trends and Predictors in the Statcast Era
👥 Authors

Aaron Slattery, Xueqing Li, Pedro Medero, Mark Tomassini, Marshall Warner, Shenhua Zhang
🧠 Overview

Modern MLB Performance explores trends and performance predictors in Major League Baseball using Statcast data from 2015 to 2024. Our team uses a variety of statistical and machine learning tools to answer key questions about how the game has evolved—especially in how players hit, pitch, and age in today’s data-rich era.

We address six main research questions involving:

    Changes in hitting trends since the Statcast era began

    Predictors of batting average

    The impact of strikeouts on offensive value

    Age-related changes in batting performance

    How pitch velocity and pitch type affect pitching success

    Predicting slugging percentage from exit velocity and hard-hit rates

📈 Key Findings

    Hard-hit and barrel rates have increased over time, while batting average slightly declined.

    Plate discipline, not contact quality, is the strongest predictor of batting average.

    High strikeout rates hurt OBP more than SLG, unless offset by high walk rates.

    Hitters peak around ages 26–30 in terms of exit velocity and hard-hit %, with clear declines after age 35.

    Pitchers with higher fastball velocities tend to post higher strikeout rates and lower expected wOBA.

    Exit velocity and hard-hit rate together explain ~32% of slugging percentage variance, making them strong offensive predictors.

🔬 Methods

Our analysis combines:

    📊 Descriptive statistics and visualizations (scatter plots, trend lines)

    📈 Mann-Whitney U tests for year-over-year comparisons

    🌲 Random forest regression to identify feature importance

    🔁 Correlation analyses using Pearson and Spearman coefficients

    📉 Linear regression for modeling slugging outcomes

    🧮 Tools: Python (pandas, sklearn, matplotlib) and R (ggplot2, dplyr, readr)

📂 Data Source

All data used in this project is publicly available from Baseball Savant, the official MLB data hub for Statcast information. The dataset includes:

    Batting and pitching metrics

    6,743 player-season entries

    42 statistical variables across 10 seasons (2015–2024)

📊 Figures and Tables

The repository includes detailed visualizations and summary tables, such as:

    📈 Figure 1: Trends in key batting stats (2015–2024)

    🌲 Figure 2: Variable importance in predicting batting average

    ⚾ Figure 3: K% vs SLG% and OBP

    📉 Figure 4: Aging curves for exit velocity and hard-hit %

    💨 Figure 5: Pitch velocity, mix, and expected performance

    🔥 Figure 6: Hard-hit % & exit velocity as predictors of slugging

    📋 Table 1: Correlations between K%, OBP, and walk rates

    📋 Table 6A: Regression model for predicting SLG

📘 Citation

If you use or reference this work, please cite our paper:

    Slattery, A., Li, X., Medero, P., Tomassini, M., Warner, M., & Zhang, S. (2024). Modern MLB Performance: Trends and Predictors in the Statcast Era.

📎 References

    Nathan, A. M., & Kagan, D. (2017). Statcast and the baseball trajectory calculator. The Physics Teacher, 55(3), 134–136.

    Sun, H.-C., Lin, T.-Y., & Tsai, Y.-L. (2022). Performance prediction in MLB by long short-term memory networks. IJDSA, 15(1), 93–104.

    Kim, S. W., et al. (2024). Inference on a zero-inflated bivariate binomial distribution applied to baseball. Statistical Modelling.

🛠️ How to Run the Code

    Clone the repository:

git clone https://github.com/your-username/statcast-mlb-analysis.git
cd statcast-mlb-analysis

Install Python dependencies:

pip install -r requirements.txt

(Optional) Run R scripts from /R_analysis folder using RStudio or command line.

Execute analysis notebooks or scripts:

    jupyter notebook analysis.ipynb

🚀 Future Work

    Incorporating biomechanical data (e.g., bat tracking) for deeper aging analysis

    Multivariate models to control for ballpark and lineup effects

    Interactive dashboards to explore Statcast metrics in real time
