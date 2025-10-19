# 📊 EDA Insights: Telecom Churn Prediction

---

## 1. Churn Rate by Gender
Both male and female customers exhibit similar churn rates, with a higher proportion of customers staying versus churning in both groups.  
This suggests that gender does not play a strong role in churn behavior within this dataset.  

![Churn Rate by Gender](images/churn_by_gender.png)

---

## 2. Model Performance: Learning Curve
The model learning curve shows consistently high ROC-AUC scores for both training and cross-validation sets, indicating the model is both accurate and stable.  
As the training sample size increases, cross-validation performance also slightly improves, demonstrating good generalization and no sign of overfitting.  

![Learning Curve](images/learning_curve.png)

---

## 3. Churn Rate by Tenure Group
Churn rate is highest among customers with the shortest tenure (0–12 months) and decreases significantly for longer-tenured groups.  
Customers remaining with the company longer are much less likely to churn, emphasizing the importance of early customer retention strategies.  

![Churn Rate by Tenure Group](images/churn_rate_tenure.png)

---

## 4. Churn Count by Tenure Group
Comparing counts, the 0–12 months tenure group has nearly equal churn/no-churn counts, while longer-tenured groups have a much greater share of non-churn customers.  
This visual reinforces the strong correlation between churn risk and tenure.  

![Churn Count by Tenure Group](images/churn_count_tenure.png)

---

## 5. Monthly Charges Distribution by Churn
Customers who churn generally have higher monthly charges compared to those who stay, with distinct peaks in the density plot indicating a relationship between billing amounts and churn likelihood.  
Price-sensitive customers appear more prone to leaving.  

![Monthly Charges Distribution by Churn](images/monthly_charges_distribution.png)

---

---

## 6. Churn Rate by Payment Method
Churn varies substantially by payment method: customers using **electronic check** have the highest churn rate, while those using **credit card (automatic)** and **mailed check** show much lower churn rates.  
This insight is crucial for designing targeted retention interventions.  

![Churn Rate by Payment Method](images/churn_rate_payment_method.png)

---

## 7. Churn Counts by Payment Method
Count analysis mirrors rate findings: **electronic check** users comprise a large portion of churners, unlike other payment types.  
Encouraging customers to switch to **auto-pay options** may be an effective strategy for improving retention.  

![Churn Counts by Payment Method](images/churn_counts_payment_method.png)

---

## 8. Model Comparison: Confusion Matrices
Confusion matrices for **XGBoost**, **Random Forest**, and **Logistic Regression** demonstrate strong predictive performance, with both true positives and true negatives outnumbering false predictions.  
XGBoost and Random Forest slightly outperform Logistic Regression in recall and precision, suggesting better handling of churn detection.  

![Confusion Matrices](images/model_confusion_matrices.png)

---

## 9. Churn by StreamingTV Feature
The **StreamingTV** feature alone does not significantly separate churners from non-churners.  
However, customers **without internet service** are much less likely to churn, indicating that **bundled service offerings** can influence customer loyalty.  

![Churn by StreamingTV Feature](images/churn_by_streamingtv.png)

---

## 10. Feature Correlations with Churn
Strong positive correlations are observed for **fiber optic internet**, **electronic check payments**, **high monthly charges**, and **paperless billing**.  
Meanwhile, **long-term contracts (two years)** and **bundled support/security services** show negative correlations with churn, identifying them as potential levers for reducing attrition.  

![Feature Correlations with Churn](images/feature_correlations.png)

---

# 📊 Essential Churn Feature Insights

---

## 🔐 Online Security & Churn
Customers **without online security** are far more likely to churn than those with protection in place.  
Notably, having *“No internet service”* aligns with very low churn, possibly due to less engagement or inactive accounts.

![Online Security & Churn](images/online_security_churn.png)

---

## 🖥️ Device Protection & Churn
A distinct drop in churn is observed for customers with **device protection services** compared to those without.  
This indicates that protection add-ons can play a key role in **retaining subscribers**.

![Device Protection & Churn](images/device_protection_churn.png)

---

## ☁️ Online Backup & Churn
The lack of **online backup** is strongly associated with higher churn rates.  
Customers who opt for backup solutions show greater loyalty — highlighting the value of **upselling digital safety features**.

![Online Backup & Churn](images/online_backup_churn.png)

---

## 📞 Multiple Lines & Churn
Subscribers with either **single or multiple phone lines** show more churn compared to those with **no phone service**.  
However, there is virtually no difference between single and multiple-line users in churn, suggesting **other factors may drive retention**.

![Multiple Lines & Churn](images/multiple_lines_churn.png)

---

## 🌐 Internet Service Type & Churn
**Fiber optic** users churn at much higher rates compared to **DSL** or **no internet** customers.  
This may reflect **service expectations** or **cost sensitivity** among fiber customers.

![Internet Service Type & Churn](images/internet_service_type_churn.png)

---

## 🧒 Dependents & Churn
Customers **without dependents** are significantly more likely to churn.  
**Family-oriented packages** could provide an effective strategy for **long-term retention**.

![Dependents & Churn](images/dependents_churn.png)

---

## 💑 Partner Status & Churn
Having a **partner** correlates with **lower churn probability**.  
Single customers are more volatile, suggesting that **family or couple bundles** could help reduce churn.

![Partner & Churn](images/partner_churn.png)

---

## 📝 Contract Type & Churn
**Month-to-month contracts** see the highest churn, while **one-year and two-year contracts** drastically reduce customer turnover.  
This underscores **contract structure** as a key factor in **churn management**.

![Contract Type & Churn](images/contract_type_churn.png)

---

## 👨‍💻 Tech Support & Churn
Availability of **tech support** is strongly linked to retention.  
Customers without tech support churn much more often, implying these services enhance **satisfaction and loyalty**.

![Tech Support & Churn](images/tech_support_churn.png)

---

## 💸 Paperless Billing & Churn
**Paperless billing** users show notably higher churn compared to those receiving paper bills.  
Further exploration could reveal if this pattern ties to **engagement levels** or **payment issues**.

![Paperless Billing & Churn](images/paperless_billing_churn.png)

---
​



