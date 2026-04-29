#  Actuarial Risk Decision Engine (Bayes + EV Model)

This project is a simple actuarial-style risk decision system built using Python.

It simulates how insurance companies make decisions using:
- Bayesian Probability
- Expected Value (EV)
- Risk-based decision making


## 🧠 What This Project Does

Given a claim with uncertain information, the model:

1. Calculates probability of fraud using Bayes Theorem
2. Estimates expected financial loss for different actions:
   - Approve claim
   - Investigate claim
3. Compares outcomes
4. Gives optimal decision (minimum expected loss)


## ⚙️ Inputs

The model takes the following inputs:

- P(Fraud)
- P(S | Fraud)
- P(S | Genuine)
- Fraud Loss
- Genuine Loss
- Investigation Cost
- Fraud Loss Recovery %


## 🧮 Concepts Used

###  Bayes Theorem
Used to update fraud probability based on observed score:

P(Fraud | S) = P(S | Fraud) × P(Fraud) / P(S)


###  Expected Value (EV)

EV = (Probability × Loss)

Used to calculate average expected loss for each decision.


###  Decision Theory

The system chooses the action with minimum expected loss:
- Approve
- Investigate


## 💡 Logic Flow

1. Input probabilities and losses  
2. Compute fraud probability using Bayes  
3. Calculate EV for Approve  
4. Calculate EV for Investigate  
5. Compare both  
6. Output best decision  


