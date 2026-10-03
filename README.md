# Lead Scoring

## Business Problem

The main objective of this project is to identify leads that are more likely to convert. This can help the business prioritize leads and focus sales efforts on leads with a higher chance of conversion.

## Approach

The data was cleaned and prepared, followed by exploratory analysis and feature selection. A Logistic Regression model was built to predict the probability of lead conversion. Different probability cutoffs were evaluated, and a final cutoff of **0.4** was selected where precision and recall were closest.

A Lead Score was then created from the model's estimated probability of conversion on a 0–100 scale.

## Model Performance

On the test set, the final model achieved:

* Accuracy: **81.96%**
* Sensitivity (Recall): **75.8%**
* Specificity: **85.99%**
* AUC: **0.879**

The overall conversion rate in the test set was **39.5%**, while the leads flagged by the model had a conversion rate of **77.9%**. This resulted in a **1.97x lift** compared with the overall conversion rate.

Overall, the model provides a useful way of ranking leads based on their estimated likelihood of conversion.
