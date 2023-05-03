# European-Call

Examine the European call option pricing data on the S&P 500. A European call option gives the holder the right (but not the obligation) to purchase an asset at a given time for a given price.

Two data sets: option_train.csv and option_test_wolabel.csv. 
1. The training data set has information on 1,680 separate options. In particular, for each option we have recorded
• Value (C): Current option value
• S: Current asset value
• K: Strike price of option
• r: Annual interest rate
• tau: Time to maturity (in years)
• BS: The Black-Scholes formula was applied to this data (using some 𝜎) to get C_pred. and If an option has C_pred – C > 0, i.e., the prediction over estimated the option value, we associate that option by (Over); otherwise, we associate that option with (Under).
2. The test data set is similar except it has only 1,120 options and is missing the Value and BS variables.

Use the training data to build statistical/ML models with
1) Value as the response (a regression problem) and then
2) BS as the response (a classification problem).
