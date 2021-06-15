# Propensity_Model

Descriptive Stats, Data analysis and Model Building for the Bank Campaign Data

The model built was a in class assignment where we used our knowledge to get the basic insights in the data, and finaly used some ensemble methods to build the Machine Learning Model to predict for the new data.

Toolkits used
* Pandas library for data Handling
* Matplotlib and Seaborn Libraries to plot the various plots 

A overview of the process.
Steps Followed:

Step 1: Data Reading and Data  Preprocesing

Step 2: Checking for missing values and handling those missing values 
  <br>The missing values in the model replaced using various techniques like mean, mode, median, KNN imputer etc

Step 3: Data Analysis 
  <br>The data was analysed to get most of the insights form the data, using pandas and matplotlib to visualize those.
  
Step 4: Data preparation for test and train
  * The coloumns required for training were selected by seeing the crelation between the features and the selected features we split into training and test set using sklearns train test split. 
  * The data has been normalized so that the model builds faster and follows our assumtion in Traditional Machine Learning algorithms.
  
Step 5: Data Modeling and Validation
  <br>After trying with various models the final model is built using RandomForest and XGBoost model. Giving better resukts than other models.
  
  
  
## Data Information
  Attribute Information:
Input variables:

*bank client data:* </br>
1 - age (numeric) </br>
2 - job : type of job (categorical: 'admin.','blue-collar','entrepreneur','housemaid','management','retired','self-employed','services','student','technician','unemployed','unknown') </br>
3 - marital : marital status (categorical: 'divorced','married','single','unknown'; note: 'divorced' means divorced or widowed) </br>
4 - education (categorical: 'basic.4y','basic.6y','basic.9y','high.school','illiterate','professional.course','university.degree','unknown') </br>
5 - default: has credit in default? (categorical: 'no','yes','unknown') </br>
6 - housing: has housing loan? (categorical: 'no','yes','unknown') </br>
7 - loan: has personal loan? (categorical: 'no','yes','unknown') </br>

*related with the last contact of the current campaign:* </br>
8 - contact: contact communication type (categorical: 'cellular','telephone') </br>
9 - month: last contact month of year (categorical: 'jan', 'feb', 'mar', ..., 'nov', 'dec') </br>
10 - day_of_week: last contact day of the week (categorical: 'mon','tue','wed','thu','fri') </br>
11 - duration: last contact duration, in seconds (numeric). </br>
    Important note: this attribute highly affects the output target (e.g., if duration=0 then y='no'). Yet, the duration is not known before a call is performed. Also, after the     end of the call y is obviously known. Thus, this input should only be included for benchmark purposes and should be discarded if the intention is to have a realistic             predictive model. </br>

*other attributes:* </br>
12 - campaign: number of contacts performed during this campaign and for this client (numeric, includes last contact) </br>
13 - pdays: number of days that passed by after the client was last contacted from a previous campaign (numeric; 999 means client was not previously contacted) </br>
14 - previous: number of contacts performed before this campaign and for this client (numeric) </br>
15 - poutcome: outcome of the previous marketing campaign (categorical: 'failure','nonexistent','success') </br>
 </br>
*social and economic context attributes* </br>
16 - emp.var.rate: employment variation rate - quarterly indicator (numeric) </br>
17 - cons.price.idx: consumer price index - monthly indicator (numeric) </br>
18 - cons.conf.idx: consumer confidence index - monthly indicator (numeric) </br>
19 - euribor3m: euribor 3 month rate - daily indicator (numeric) </br>
20 - nr.employed: number of employees - quarterly indicator (numeric) </br>

*Output variable (desired target):* </br>
21 - y - has the client subscribed a term deposit? (binary: 'yes','no') </br>

  
