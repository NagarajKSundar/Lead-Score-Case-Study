# Lead-Score-Case-Study
# Problem Statement :

An education company named X Education sells online courses to industry professionals. On any given day, many professionals who are interested in the courses land on their website and browse for courses. 

The company markets its courses on several websites and search engines like Google. Once these people land on the website, they might browse the courses or fill up a form for the course or watch some videos. When these people fill up a form providing their email address or phone number, they are classified to be a lead. Moreover, the company also gets leads through past referrals. Once these leads are acquired, employees from the sales team start making calls, writing emails, etc. Through this process, some of the leads get converted while most do not. The typical lead conversion rate at X education is around 30%. 

Now, although X Education gets a lot of leads, its lead conversion rate is very poor. For example, if, say, they acquire 100 leads in a day, only about 30 of them are converted. To make this process more efficient, the company wishes to identify the most potential leads, also known as ‘Hot Leads’. If they successfully identify this set of leads, the lead conversion rate should go up as the sales team will now be focusing more on communicating with the potential leads rather than making calls to everyone. A typical lead conversion process can be represented using the following funnel:

![image](https://github.com/NagarajKSundar/Lead-Score-Case-Study/assets/116784388/e7f0dbe3-d5d0-49dd-bb24-de5319ab63e8)

As you can see, there are a lot of leads generated in the initial stage (top) but only a few of them come out as paying customers from the bottom. In the middle stage, you need to nurture the potential leads well (i.e. educating the leads about the product, constantly communicating etc. ) in order to get a higher lead conversion.

X Education has appointed you to help them select the most promising leads, i.e. the leads that are most likely to convert into paying customers. The company requires you to build a model wherein you need to assign a lead score to each of the leads such that the customers with a higher lead score have a higher conversion chance and the customers with a lower lead score have a lower conversion chance. The CEO, in particular, has given a ballpark of the target lead conversion rate to be around 80%.

# Data:
You have been provided with a leads dataset from the past with around 9000 data points. This dataset consists of various attributes such as Lead Source, Total Time Spent on Website, Total Visits, Last Activity, etc. which may or may not be useful in ultimately deciding whether a lead will be converted or not. The target variable, in this case, is the column ‘Converted’ which tells whether a past lead was converted or not wherein 1 means it was converted and 0 means it wasn’t converted. You can learn more about the dataset from the data dictionary provided in the zip folder at the end of the page. Another thing that you also need to check out are the levels present in the categorical variables. Many of the categorical variables have a level called 'Select' which needs to be handled because it is as good as a null value (think why?).

# Goals of the Case Study:
There are quite a few goals for this case study:

Build a logistic regression model to assign a lead score between 0 and 100 to each of the leads which can be used by the company to target potential leads. A higher score would mean that the lead is hot, i.e. is most likely to convert whereas a lower score would mean that the lead is cold and will mostly not get converted.
There are some more problems presented by the company which your model should be able to adjust to if the company's requirement changes in the future so you will need to handle these as well. These problems are provided in a separate doc file. Please fill it based on the logistic regression model you got in the first step. Also, make sure you include this in your final PPT where you'll make recommendations.

# Table of Contents
General Info
Technologies Used
Conclusion

# General Information:
# Business Understanding
- Understand the requirements of the Assignment.

# Data Understanding
- Understand the datasets provided.

# Data Cleaning & Manipulation
- Clean the data and perform some manipulation

# Data Visualization
- Perform EDA to gain a better understanding of the dataset and its various variables. This may include summary statistics, data visualizations, and data distribution analysis.
- Check the correlation between the variables to understand the relationships and dependencies among them. You can create correlation matrices or visualizations to help with this analysis.

# Data Preparation
- Create dummy variables for all the categorical features to convert them into a numerical format suitable for modeling.
- Divide the data into training and testing sets to facilitate model training and evaluation.
- Perform data scaling to standardize or normalize the numerical features as necessary for the chosen algorithms.
- Divide the data into dependent and independent variables, separating the target variable from the features for modeling.

# Data Modeling & Evaluation
- Create a Linear Regression model using a mixed approach that combines Recursive Feature Elimination (RFE) and Variable Inflation Factor (VIF) or p-value selection methods.
- Ensure that the various assumptions of linear regression are checked, including linearity, independence of errors, homoscedasticity, and normality of residuals.
- Evaluate the model's performance by checking metrics such as Accuracy, Sensitivity, Specificity, Precision, and Recall.
- Report the final Linear Regression model, including the selected features, coefficients, and a summary of the model's performance.

# Technologies Used
- Jupyter Notebooks
- Anaconda Navigator
- GitHub
- Matplotlib
- Seaborn
- NumPy
- Pandas
- Statsmodels
- Scikit-learn

# Conclusions :
These are the key variables that play a significant role in the conversion rate

Lead Source_Welingak Website                            6.508686
Lead Source_Reference                                   4.233370
Total Time Spent on Website                             3.417487
What is your current occupation_Working Professional    2.648638
Lead Origin_Lead Import                                 1.754495
Lead Source_Olark Chat                                  1.399249
Specialization_Others                                  -0.426853
Last Notable Activity_Email Opened                     -1.425355
Last Notable Activity_Page Visited on Website          -1.683992
Do Not Email                                           -1.867923
Last Notable Activity_Email Link Clicked               -1.891884
Last Notable Activity_Modified                         -2.105825
Last Notable Activity_Olark Chat Conversation          -2.730931

# Recommendations for the company/CEO :
- The company should prioritize leads from the sources "Welingak Websites" and "Reference", as they are more likely to result in conversions.

- Leads who have spent a significant amount of time on the company's websites should be a primary focus, as their extended engagement indicates a higher conversion potential.

- Targeting working professionals among the leads is advisable, as they tend to have a greater likelihood of conversion.

- Special attention should be given to leads sourced from "Lead Import", as they demonstrate a higher chance of conversion.

- It is recommended to focus efforts on leads sourced through "Olark Chat", as these leads are more likely to convert.

- It is advisable for the company to refrain from contacting leads whose most recent interactions were categorized as "Email Opened", "Page Visited on Website", "Email Link Clicked", "Modified", or "Olark Chat Conversation", as these activities are less likely to result in conversions.





