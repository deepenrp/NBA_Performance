# NBA Performance

How do we measure which player is better than the next or better question how do we measure how much overall success a player brings to their team as this will determine which player will eventually win the most valuable player award at the end of the season?

According to Basketball-Reference, win shares is a metric that estimates the number of wins a player produces for his team throughout the season. We believe win shares is a very good indicator but how do we predict win shares and what is it based on - Personal Success or basic stats – ex: number of points you score, assist or rebound? Advances Stats – ex: how well you contribute to the team? Or rather a combination of basic and advanced metrics?

What criteria matters most in making your MVP decision? Answers by some of nba sports writers/analyst
  - Steve Aschburner: The MVP is the best player on the team with the best record.
  - Fran Blinebury: Consistent individual excellence combined with team leadership and more than a few moments of transcendent brilliance.
  - John Schuhmann: My vote went to the individual who had the biggest effect on why a good team was good.
   - Sekou Smith: I've said all along that there's a complicated matrix of factors that go into making this vote.
   - Ian Thomsen: I love this award because it’s all about value: who has done the most for his team?
  - Lang Whitaker: I'm doing my best to keep it simple: Value.

Source: https://www.nba.com/article/2017/04/12/blogtable-what-criteria-matters-most-making-mvp-decision


### Data Sources:

Web Scrape 
- Scrape data for 2018-2019 and 2019-2020 season: https://www.basketball-reference.com/

NBA Fantasy
-


## Technologies used:
```
Pandas
Matplotlib
Seaborn
Sklearn
Plotly
```

## Data Clean Up Process:

Data Collection:
  * Web Scrape from Basketball Reference (www.basketball-reference.com)
    * 2018-2019
      * Basic Stats
      * Advanced Stats
      * Merge them into one
    * 2019-2020
      * Basic Stats
      * Advanced Stats
      * Merge them into one

Feature Selection:

  * Find the most important feature(s) to be used for the model
    * Random Forest Regression
    * Correlation Matrix (Pearson R-Square Correlation)
      * Create a Heatmap

Supervised Machine Learning Model
  * Training and Validation
    * Train –
      * Year 2018-2019
      * Multi-Linear Regression
    * Validate/Test –
      * Year 2019-2020 (Current Season)
      * Check our predicted win shares values against the actual
