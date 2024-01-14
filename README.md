# BayesianBandit
## About this project
This project illustrates the Bayesian bandit algorithm (also known as Thompson sampling), which is an algorithm used to determine the best strategy among multiple choices while balancing between maximizing the reward and collecting new information that could increase future rewards. The codes are written in the context of email marketing for e-commerce. Imagine that you are running an e-commerce company and you have noticed that many customers place items in their shopping basket but do not proceed with the purchase. You want to test if sending a reminder email about the incomplete transaction would help them proceed to purchase, and if so, determine the optimal timing for sending the email. Specifically, you want to test five different timing strategies: 30 minutes later, 2 hours later, 1 day later, 3 days later, and 1 week later.

## Contents
**Bayesian_bandit_email_timing_experiment.ipynb**: Contains the Byesian Bandit algorithm explaining how it learns the best strategy assuming the following purchase rates: 0.0001 for not sending an email, 0.05 for 30 minutes, 0.02 for 2 hours, 0.01 for 1 day, 0.01 for 3 days, and 0.001 for a week later. 

**requirements.txt**: Shows necessary package versions to run the above file.

## Results
After sending 2000 emails, the algorithm correctly identified the two best optimal strategies: 30 minutes and 2 hours. After that, the algorithm is more likely to choose these strategies. One of the benefits of Bayesian A/B testing is the ability to stop the experiment at any time.
