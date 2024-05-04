## Logistic Regression Analysis
We want to look specifically at variables' influence on Steam’s determination of comments' positivity. Using a sample dataset we test logistic regression’s assumptions (linearity assumption, outliers, and multicollinearity), then run a stepwise variable selection to choose the most influential factors from the factors we chose. Using a logistic regression model for parallel computing on every language file we found that the chosen variables’ p-value are all small but some estimates are also small. It's found that ‘number of likes on a comment’ has a negative estimate for all languages, indicating people tend to like negative comments globally. This potentially questioned the credentials of steam’s determination of the comments’ positivity. We also found that players tend to give positive comments if they purchase the game.

## Linear Regression Analysis

In order to assess the determinants influencing the helpfulness score of reviews, a linear regression analysis was conducted using "weighted score"(helpfulness score) as the dependent variable and several predictors including playtime, comment count, and the number of votes. The analysis employed 29 parallel processing tasks (20 minutes run time, less than 1GB memory and disk space) on split data to identify significant predictors and to quantify their occurrences. A threshold of significance was established at an 80% occurrence rate across the split files.

The results revealed that the variables representing author's last playtime, the number of comments(comment_count), the timestamp of review(timestamp_created), and the number of votes (votes_up) consistently emerged as significant in over 80% of the datasets analyzed. Consequently, these factors were deemed influential in determining review helpfulness. The analysis further suggested a positive correlation between reviews that were posted soon after the application was launched, and those that garnered a high number of votes and comments, with the perceived helpfulness of the review on the Steam platform.

Linear Regression Analysis and pre_logistic.Rmd is runned in local machine (stepwise variable selection & assumption tests)

