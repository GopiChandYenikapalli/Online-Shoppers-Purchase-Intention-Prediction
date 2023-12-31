# Online-Shoppers-Purchase-Intention-Prediction

![image](https://github.com/GopiChandYenikapalli/Online-Shoppers-Purchase-Intention-Prediction/assets/124816585/3d8e9880-dc53-488a-85e3-4b98b11b58e8)


<img width="100%" alt="image" src="https://github.com/GopiChandYenikapalli/Online-Shoppers-Purchase-Intention-Prediction/assets/124816585/4c8468dc-0979-4b49-bdfa-744143de8033">

# Business Scenario:

A new company has entered the market and is looking to increase its sales by launching marketing campaigns to reach potential customers. The company is focused on building its own brand and wants to ensure that it is targeting the audience and ready to spend its maximum marketing budget.

To achieve this, the company plans to use a machine learning model to identify potential customers who are likely to make a purchase on their website. The company has collected data on visitors to their website, including the number of pages viewed, the time spent on the website, the type of visitor, and the location of the visitor.

# Column Descriptions:

1. Administrative: The number of pages of administrative information visited by the user.

2. Administrative_Duration: The total time spent by the user on the administrative pages.

3. Informational: The number of pages of informational content visited by the user.

4. Informational_Duration: The total time spent by the user on the informational pages.

5. ProductRelated: The number of pages of product-related content visited by the user.

6. ProductRelated_Duration: The total time spent by the user on the product-related pages.

7. BounceRates: The percentage of visitors who enter the website and leave without viewing any other pages.

8. ExitRates: The percentage of visitors who leave the website after viewing a page.

9. PageValues: The average value of the pages viewed by the user before the purchase.

10. SpecialDay: The closeness of the visit to a special day like Mother's Day or Valentine's Day.

11. Month: The month of the year when the user visited the website.

12. OperatingSystem: The operating system used by the user.

13. Browser: The browser used by the user.

14. Region: The geographical region of the user.

15. TrafficType: The type of traffic source from which the user arrived at the website.

16. VisitorType: The type of visitor - returning or new.

17. Weekend: A binary value indicating whether the visit occurred on a weekend or not.

18. Revenue: The target variable indicating whether the user made a purchase or not (1 for purchase, 0 for no purchase).

Note that this dataset is a combination of web analytics data and survey data, and the columns represent various attributes of the user's browsing behavior on a large online retailer in Turkey.

# Performance metrics Identification

### As this company is new to the market and wants to spend more on marketing campaigns to reach as many potential customers, building its own brand and focusing on product sales.

True Positives (TP): Users who were correctly identified by the model as potential customers who made a purchase.

False Positives (FP): Users who were incorrectly identified by the model as potential customers who made a purchase, but in reality, they did not.

True Negatives (TN): Users who were correctly identified by the model as non-potential customers who did not make a purchase.

False Negatives (FN): Users who were incorrectly identified by the model as non-potential customers who did not make a purchase, but in reality, they did.


# Selecting performance metrics

Clearly, our data set is imblanced and the majority class is 0 (not purchased) and the minority class is 1 (purchased). If we choose accuracy, it will focus on the majority class, which is not good in our case. Then we need to focus on Recall, precision, and F1 score.

Recall and precision scores depend on the specific goal of the analysis and the trade-off between identifying all positive instances (high recall) and minimizing the number of false positives (high precision).

To minimize the number of false positives, even if it means potentially missing some positive instances, precision should be the primary metric to focus on. High precision means that the model is able to correctly identify positive instances with a high degree of certainty, which is important for minimizing the cost of false positives, such as wasting resources on marketing campaigns to non-interested customers. However, the company is more concerned with not missing out on potential customers and wants to minimize False Negatives (FN), they prioritize maximizing Recall, which measures the proportion of true positives among all actual positive cases (TP / (TP + FN)). A higher Recall score indicates that the model is better at identifying all positive cases, even if it means making more false positive predictions, which means identifying all users who are likely to make a purchase, regardless of the number of false positives.

# Recall scores
**************************************
Logistic Regression deafult:0.7454545454545455

Logistic Regression Random Search:0.7454545454545455

Logistic Regression Grid Search:0.7454545454545455

**************************************
SVM Linear deafult:0.730909090909091

SVM Linear Random Search:0.730909090909091

SVM Linear Grid Search:0.730909090909091

**************************************

SVM rbf deafult:  0.7490909090909091

SVM rbf Random Search:0.7345454545454545

SVM rbf Grid Search:0.7327272727272728

**************************************

SVM Poly deafult: 0.7345454545454545

SVM Poly Random Search:0.7163636363636363

SVM Poly Grid Search:0.7163636363636363

**************************************

Decision Tree deafult:0.5636363636363636

Decision Tree Random Search:0.8490909090909091

Decision Tree Grid Search:0.8345454545454546

**************************************

ANN deafult:      0.6290909090909091

ANN Random Search:0.649090909090909

ANN Grid Search:  0.8545454545454545

**************************************

DNN with Random Search:0.8036363636363636

DNN deafult :     0.7981818181818182

DNN with Random Grid Search:0.7981818181818182

WDNN:             0.82
**************************************


# Contact details
If you've enjoyed browsing through my portfolio or would like to discuss potential work opportunities or collaborations, please reach out to me via email <stong/>gopichandyenikapalli@usf.edu <strong/> or https://www.linkedin.com/in/gopichand-yenikapalli-usf/

I'm always excited to connect with new people in the industry and explore potential partnerships or projects together. I look forward to hearing from you soon!
