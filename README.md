# cardiovascular-risk-prediction

 ![image](https://user-images.githubusercontent.com/103834221/209559634-c07b9e4d-ebe8-4788-b39d-c5b5cd17decb.png)

## Introduction:

Coronary heart disease is a type of heart disease where the arteries of the heart cannot deliver enough oxygen-rich blood to the heart. Coronary artery disease affects the larger coronary arteries on the surface of the heart. Another type of heart disease, called coronary microvascular disease, affects the tiny arteries in the heart muscle. Coronary microvascular disease is more common in women. Symptoms of coronary heart disease may be different from person to person, even if they have the same type of coronary heart disease.
The dataset is from an ongoing cardiovascular study on residents of the town of Framingham, Massachusetts. The classification goal is to predict whether the patient has a 10-year risk of future coronary heart disease (CHD). The dataset provides the patient's information. It includes over 4,000 records and 15 attributes. Each attribute is a potential risk factor. There are both demographic and behavioral and medical risk factors.

## Dataset :
- Demographic: 
• Sex: male or female("M" or "F")

• Age: Age of the patient;(Continuous - Although the recorded ages have been truncated to whole numbers, the concept of age is continuous)

• is_smoking: whether or not the patient is a current smoker ("YES" or "NO")

• Cigs Per Day: the number of cigarettes that the person smoked on average in one day.(can be considered continuous as one can have any number of cigarettes, even half a cigarette.) 

Medical( history)

• BP Meds: whether or not the patient was on blood pressure medication (Nominal)

• Prevalent Stroke: whether or not the patient had previously had a stroke (Nominal)

• Prevalent Hyp: whether or not the patient was hypertensive (Nominal)

• Diabetes: whether or not the patient had diabetes (Nominal) Medical(current)

• Tot Chol: total cholesterol level (Continuous)

• Sys BP: systolic blood pressure (Continuous)

• Dia BP: diastolic blood pressure (Continuous)

• BMI: Body Mass Index (Continuous)

• Heart Rate: heart rate (Continuous - In medical research, variables such as heart rate though in fact discrete, yet are considered continuous because of large number of possible values.)

• Glucose: glucose level (Continuous) Predict variable (desired target)

## Approach :

Data cleaning and preprocessing: Here I checked and dealt with missing and duplicate variables from the data set as these can grossly affect the performance of different machine learning algorithms (many algorithms do not tolerate missing data).

Exploratory Data Analysis: Here I wanted to gain important statistical insights from the data and the things that I checked for were the distributions of the different attributes, correlations of the attributes with each other and the target variable and I calculated important odds and proportions for the categorical attributes.

Feature Selection: Since having irrelevant features in a data set can decrease the accuracy of the models applied, I used Tree-based: SelectFromModel which is an embedded method that uses algorithms that have built-in feature selection methods which were later used to build different models.

Model development and comparison: I used four classification models, i.e., Logistic Regression,K-nearest neighbors , Decesion tree , Random Forrest classifier ,support vector machine,Light Gradient Boosting Machine With Grid Search CV,Random Forest Classifier Using Randomised Search CV After which I compared the performance of the models using their recall and F1 score . I then settled with the best performing model.

## Conclusion:
7 models were used in the project namely

- Logistic Regressor.
- K-Nearest Neighbour Classifier.
- Decision Tree Classifier.
- Random Forest Classifier.
- Support Vector Machines.
- Light Gradient Boosting Machine With Grid Search CV.
- Random Forest Classifier with Randomised Search CV.

The models that could can be deployed according to our study is Random Forest Classifier with Accuracy-0.908 ,Precision- 0.941, Recall- 0.941.

Better model can be developed that can predict the risk of coronary heart disease.

With the help of the experts we can engineer an extensive amount of variable that could make our prediction more accurate.

Hence, we can say that Machine Learning can help save lives of many and help them to switch over to a healthy lifestyle to chop off any health related issue.
