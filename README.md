# Capstone - Predicting the Philadelphia 76ers' Success

#### By David Cortes

## Problem Statement

This capstone aims to build a regression model with Houston Rockets data in order to predict how many three-point field goals the Philadelphia 76ers make in the upcoming NBA season.

## Data

The Houston Rockets and Philadelphia 76ers data used in this project was scraped from basketball-reference.com. Once the data was craped, they were transferred to CSV files.
- Training data: game logs for each player on the 2017-2018 Rockets roster
- Testing data: game logs for each player on the 2020-2021 Sixers roster

## Modeling

Linear, Ridge, and Lasso regression models were each tested.
- PolynomialFeatures was used (degree=2)
- Mean cross-val score:
 - Lasso: 0.79696671
 - Ridge: 0.798621953
 - Linear: 0.8

The Lasso Regression model returned the best accuracy score.
- Training Score: 0.999241585099331
- Testing Score: 0.997952083858883

## Findings and Conclusion

- The Lasso model turned out very accurate, with a score of over 99%
- Using data from the Sixers’ first 18 games, the model was able to predict about 161 three-pointers
- I'm hopeful that this data and model can be useful for purposes like training, fantasy basketball, etc.

## Next Steps

- Find a way to gather data that shows the number of field goals made from right under the basket.
- Regularly update the testing data as the 2020-2021 NBA season continues.
- Feature engineer more advanced stats(3-point attempt rate,  turnover percentage, etc.)
- Increase the size of the training data (combine two or three years of Houston Rockets game logs)
- Explore more models like ElasticNet

## Works Cited

- https://www.basketball-reference.com/
- https://github.com/vishaalagartha/basketball_reference_scraper
- https://pypi.org/project/Unidecode/