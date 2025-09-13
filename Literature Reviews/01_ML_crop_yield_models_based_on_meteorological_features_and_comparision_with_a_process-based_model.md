# Literature Review

## ML Crop Yield Models Based on Meteorological Features and Comparision with a Process-Based Model

### Definitions/Unfamiliar Terms:

- leaving-one-year-out approach: used when k-fold cross validation would break a natural temporal order and lead to
  infomration leakage. In each iteration, train all years except one and use the left-out year as the test set
- Process based crop model (PBM): Uses biological/chemical/physical equations for the basis of the model instead of
  subject matter agnostic formulas

### Abstract 

- As climate change exacerbates the volatility of crop yield, developing models which can accurately predict yields is
  very important for short-term and long-term planning. 
- Authors train/validate multiple ML models using the leaving-one-year-out approach and compare the results to the PBMs
- Found that LSTM with attention outperforms other ML and PBM model (explains 73% of the spatiotemporal variance)

### Introduction

- Most studies in the past used classical statistical approaches like multi-variate regression [pot. study #1](https://www.nature.com/articles/s43016-020-00165-w) [pot. study #2](https://www.sciencedirect.com/science/article/pii/S0048969720314066?via%3Dihub)
    - However, they used meteorological statistics during growing season, which cannot capture impact of extreme weather
      conditions during critical stages of crop development that may have a disproportionate impact on crop yield.
    - Also, historically uncprecedented events may not follow the patterns extrapolated by the classical approaches
- ML/Deep learning emerged as an alt. approach: [pot. study #3](https://www.sciencedirect.com/science/article/pii/S0168169920302301?via%3Dihub)
    - CNN and LSTM are most frequently used
- 4th paragraph in the introduction gives a summary of methods attempted
- Authors developed LSTM with attention to account for both dynamic and static features. Incorporate static features to
  calculate the attention.
