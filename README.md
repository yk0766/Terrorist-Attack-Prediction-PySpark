# Terrorist Attack Prediction

## Problem Statement
Terrorism is defined in the Oxford dictionary as the unlawful use of violence and intimidation, especially against civilians, in the pursuit of political aims. In recent years, terrorist activities have been increasing throughout the world. According to a survey, about 68 thousand people lose their lives annually and 220 million people are affected every year due to natural (famine, earthquakes, tsunamis) and man-made calamities (terrorism). Although natural calamities have been constant, the terrorist activities have significantly increased over the years.
 

## Goal 
The main objective of the project is to analyze terrorist activities around the globe and predict the success of a terrorist attack using different machine learning approaches.

<img width="801" alt="image" src="https://user-images.githubusercontent.com/99356847/204161761-2e2c956e-ea4d-46d0-8746-081fd0ff2fcc.png">



## Dataset
We will be using Global Terrorism Database which is an open- source database including information on terrorist attacks around the world from 1970 through 2017. The GTD includes systematic data on domestic as well as international terrorist incidents that have occurred during this time period and now includes more than180,000 attacks. The database is maintained by researchers at the National Consortium for the Study of Terrorism and Responses to Terrorism(START). 

•	Instances – 201183

•	Variables – 68

•	Target variables (success) – To predict the success of terrorist attacks across the globe

  Success Values
  
  Successful attack - 1
  Unsuccessful attack - 0 (failure to implement the attack)
  

•	Source - https://www.start.umd.edu/gtd/

## Dataflow Diagram
<img width="600" alt="image" src="https://user-images.githubusercontent.com/99356847/204161356-b17a320f-ea90-4e6c-b31c-23317b5ab932.png"> 

## Exploratory Data Analysis
      
•	Explored relationship among the variables and selected important variables using correlation matrix.

•	Displayed class imbalance with help of a count plot and understood other features impact on terrorist attacks using bar plot.

•	Analyzed variable distribution with help of histograms.

<img width="550" alt="image" src="https://user-images.githubusercontent.com/99356847/204161419-68a2ad67-ecf4-4eaf-ba63-ae7a3fe8326e.png"> <img width="550" alt="image" src="https://user-images.githubusercontent.com/99356847/204161465-2b68470e-8dab-46a0-bd9d-f05034edf4ef.png">


## Insights obtained after EDA
•	It was observed that most terrorist attacks are happening in Asian countries as these countries have many internal terrorist groups.

•	It was observed that private property, military, and police are most targeted entity in these attacks.

•	It is seen that number of attacks have been reducing with years due to latest advancement in technology and Artificial intelligence.

<img width="387" alt="image" src="https://user-images.githubusercontent.com/99356847/204161540-c61060e4-71e9-4143-bede-a82a6f965310.png"> <img width="392" alt="image" src="https://user-images.githubusercontent.com/99356847/204161556-c53e6a2a-8535-4847-8d8a-d31475aa2a31.png">


## Preprocessing
•	Removed outliers and replaced null values present in the column.

•	Filtered data before 2012 due to unorganized data collection as mentioned in the source website from where the dataset is taken.

•	Used weight balancing to handle the problem of class imbalance.


## Machine Learning Model and Evaluation

• Naïve Bayes

• Random Forest

• Logistic Regression

• Gradient Boost

<img width="1000" alt="image" src="https://user-images.githubusercontent.com/99356847/204161712-1dfa75b2-a881-498b-b12b-e0921022cfe5.png">


## Conclusion
Gradient Boost shows the highest accuracy, AUC, and F-1 score. The performance of the model has been further improved by preprocessing the data even further like removing outliers, transforming the skewed features, etc. One of the major takeaways from the project is that accuracy is not the only metric we need to look forward to while we are building the model, there are parameters that need careful consideration based on the use case. In the future, we could build ensemble models to get higher accuracy, precision, and AUC for the data. Additionally, the research could be extended to building multiclass classification, this will help in identifying the regions with high, medium and low risk of attacks such that preventive measures can be taken accordingly. 
