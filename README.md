# Loan Default Detector

<details>
<summary><b>Check out my other projects!</b></summary>
  
[Demand Forecasting](https://github.com/lexie21/demandforecasting)

[Movie Recommender](https://github.com/lexie21/movierecommender)

</details>

## Table of Contents
- [Introduction](#introduction)
- [EDA](#exploratory-data-analysis)
- [Modeling](#modeling)

## Introduction

<b>What this project is about?</b>

- Project Scope

  Loan default prediction is critical for financial institutions to minimize risk and make informed lending decisions. This project focuses on building a machine learning model to detect potential loan defaulters based on historical borrower data. The objective is to analyze key borrower attributes—such as income, credit history, loan amount, and repayment behavior—to identify patterns that indicate a higher risk of default.

  By accurately predicting defaulters, this project aims to help financial institutions improve risk assessment, reduce losses, and optimize lending strategies. These insights can also enhance customer profiling and responsible lending practices.

<b>What I did?</b>

- EDA

  Analyzed default rates across different dimensions (e.g., borrower demographics, loan type) to identify key risk factors.
  Examined default trends over time to detect seasonality or economic influences.
  
- Recommendation Engine
  
  Applied techniques to address class imbalance for better default detection.
  Built predictive models using Gradient Boosting and Random Forest.
  Implemented a Feedforward Neural Network to capture complex relationships.

## Exploratory Data Analysis

<h3>Metrics and Dimensions</h3>

- **Average default amount:** average loss incurred from each default
- **Default ratio:** proportion of default cases out of all loans
- **Employment status:** 12 types in total
- **House type:** shared usage, private-only, regular, company-olny and unknown

<h4>Overall Stats:</h4>

|Year | Application Month | #Defaults | Sum Default Amount | Sum Loan Amount | Default Ratio | Average Default Amount| Max Amount|
|------------|----------|--------|--------|--------|--------|--------|--------|
|   2020     | 10 | 0.807  |0.807  |0.807  |0.807  |0.807  |0.807  | 


This table provides valuable insights into the bank's performance. On average, the bank approves over 1,800 to 1,900 loans per month, with October 2020 seeing a significant spike, doubling the usual amount. The default ratio remains consistent at 20% of all loans, with the average amount per default case exceeding 1,000. Overall, defaults account for about 22-25% of the entire loan portfolio, and 2021 experienced much higher losses compared to the previous year.

Several key observations stand out: While October 2020 and January 2021 show some of the highest absolute numbers of defaults, the average amount per default is relatively low, around 1,150. In contrast, November 2020 saw the highest average default amount, at 1,370, despite having the fewest default cases both in absolute numbers (276) and percentage (19%). Lastly, it appears the bank has a cap of 3,000 on its loan amounts, which should be further investigated, as this limit may not align with industry standards.

<h4>Employment Status:</h4>

![Alt Text](https://github.com/lexie21/loandefaulter/blob/main/employment_status.png)

<h4>House Type:</h4>

![Alt Text](https://github.com/lexie21/loandefaulter/blob/main/house_type.png)


<h3>Summary of Insights</h3>

<h3>Recommendations & Next Steps</h3>

## Modeling

| Model | AUC | AP |
|------------|----------|--------|
| Random Forest       | 0.880 | 0.807  | 
| Gradient Boosting       | 0.866    | 0.706   | 

![Alt Text](https://github.com/lexie21/loandefaulter/blob/main/ML_curves.png)
![Alt Text](https://github.com/lexie21/loandefaulter/blob/main/DL_curve.png)

