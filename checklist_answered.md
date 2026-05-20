# Feature Engineering Checklist

## 1. General Structure of the Dataset

**Q1.** Does your dataset contain variables that are not immediately usable by a machine learning algorithm?  
Yes [x]  No [ ]  Not sure [ ]

**Q2.** Are there columns that represent dates, categories, texts, codes, or identifiers?  
Yes [x]  No [ ]  Not sure [ ]

**Q3.** Are some variables useful in theory, but poorly represented in their current form?  
Yes [x]  No [ ]  Not sure [ ]

**Q4.** Are there variables that may need to be combined, transformed, or simplified?  
Yes [x]  No [ ]  Not sure [ ]

## 2. Numerical Features

**Q5.** Do numerical variables have very different scales?  
Yes [x]  No [ ]  Not sure [ ]

**Q6.** Are some numerical variables strongly skewed?  
Yes [x]  No [ ]  Not sure [ ]

**Q7.** Are there extreme values that may distort the analysis?  
Yes [x]  No [ ]  Not sure [ ]

**Q8.** Are some numerical variables difficult to interpret in their raw form?  
Yes [x]  No [ ]  Not sure [ ]

**Q9.** Do scatter plots suggest nonlinear relationships?  
Yes [ ]  No [ ]  Not sure [x]

## 3. Categorical Features

**Q10.** Does your dataset contain nominal categorical variables?  
Yes [x]  No [ ]  Not sure [ ]

**Q11.** Does your dataset contain ordinal categorical variables?  
Yes [x]  No [ ]  Not sure [ ]

**Q12.** Do some categorical variables have many distinct categories?  
Yes [ ]  No [x]  Not sure [ ]

**Q13.** Are some categories too rare to be analytically useful?  
Yes [ ]  No [x]  Not sure [ ]

**Q14.** Would numerical encoding introduce a false order among categories?  
Yes [x]  No [ ]  Not sure [ ]

## 4. Date and Time Features

**Q15.** Does your dataset contain dates or timestamps?  
Yes [ ]  No [x]  Not sure [ ]

**Q16.** Is the time elapsed since an event more meaningful than the date itself?  
Yes [ ]  No [x]  Not sure [ ]

**Q17.** Are there seasonal, weekly, or cyclical patterns?  
Yes [ ]  No [x]  Not sure [ ]

**Q18.** Are previous values relevant to current outcomes?  
Yes [ ]  No [x]  Not sure [ ]

## 5. Text Features

**Q19.** Does your dataset contain open-ended text responses, comments, titles, descriptions, or reviews?  
Yes [ ]  No [x]  Not sure [ ]

**Q20.** Could text length, word count, or frequency of terms be informative?  
Yes [ ]  No [x]  Not sure [ ]

**Q21.** Are specific words or expressions analytically relevant?  
Yes [ ]  No [x]  Not sure [ ]

**Q22.** Is semantic similarity between texts important?  
Yes [ ]  No [x]  Not sure [ ]

**Q23.** Are texts too noisy or inconsistent?  
Yes [ ]  No [x]  Not sure [ ]

## 6. Redundancy and Dimensionality

**Q24.** Do some variables measure almost the same thing?  
Yes [ ]  No [x]  Not sure [ ]

**Q25.** Are some variables highly correlated with each other?  
Yes [x]  No [ ]  Not sure [ ]

**Q26.** Does your dataset have many columns compared to the number of observations?  
Yes [ ]  No [x]  Not sure [ ]

**Q27.** Did encoding create many sparse columns?  
Yes [ ]  No [x]  Not sure [ ]

**Q28.** Are some variables theoretically irrelevant to your research question?  
Yes [ ]  No [ ]  Not sure [x]

## 7. Connection with Future Machine Learning Models

**Q29.** Would you use kNN, SVM, k-Means, DBSCAN, or PCA?  
Yes [ ]  No [ ]  Not sure [x]

**Q30.** Would you use linear or logistic regression?  
Yes [x]  No [ ]  Not sure [ ]

**Q31.** Would you use decision trees?  
Yes [x]  No [ ]  Not sure [ ]

**Q32.** Would you use clustering?  
Yes [ ]  No [ ]  Not sure [x]

**Q33.** Would you prioritize interpretability?  
Yes [x]  No [ ]  Not sure [ ]

## Final Decision

Moderate need for feature engineering [x]
Low need for feature engineering [ ]
High need for feature engineering [ ]

## Short Written Answer

Based on my exploratory analysis, my dataset requires moderate feature engineering. The main reasons are the presence of categorical/ordinal variables that still need proper encoding, numerical variables with different scales, and some skewness/outliers (especially in tutoring-related counts). The most relevant operations would be one-hot/ordinal encoding, feature scaling, and robust outlier treatment, because these steps improve model stability, comparability, and predictive performance across different algorithms. Before applying machine learning algorithms, I should prioritize building a clean preprocessing pipeline (encoding + scaling + outlier strategy) and checking feature redundancy/correlation to avoid multicollinearity and unnecessary variables.
