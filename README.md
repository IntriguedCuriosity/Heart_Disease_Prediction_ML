## Heart Disease Prediction Using Machine Learning 

##### Summary: 
In this project, we have successfully built a Machine Learning model that will keep getting better 
as we provide more data to predict the likelihood of heart disease within 10 years. 
After testing multiple models, Logistic Regression (Baseline Model), Decision Tree Classifier 
(Interpretable), Random Forest Classifier with and without tuned HyperParameters, XGBClassifier, 
Support Vector Machine (SVM), & Neural Network (Feedforward) (Deep Learning Approach) we 
finalized Random Forest Classifier as our best-performing model with the accuracy of 77%. 
Even though Random Forest had an improved accuracy, all models struggled to have the good 
Precision, recall and F1-score. This meant all models were biased towards predicting "No Heart 
Disease" (class 0) this would have been true, if we had not done resampling to have equal 
population of class 1 & class 0 but with sampling as well we struggled to have good metrics even 
after tuning hyperparameters. XGBClassifier which uses Gradient Boosting, meaning it focuses on 
mistakes from previous trees as well didn’t managed to get a good result. 
This was seen because we had several features which made the model complex, and also some of 
the important feature like family history of heart disease as a factor, exercise & dietary habits 
could have increased our model overall. 
In the end, we have the model function ready to be used by medical team by feeding inputs to 
predict the possibilities and hence create awareness among patients, so they can rectify and make 
lifestyle changes for a better living. 




``Attributes of our Dataset:``

I have divided the columns details as per their domain for having better understanding 

 Demographic: 
    
    o Sex: male or female(Nominal) 
    o Age: Age of the patient;(Continuous - Although the recorded ages have been 
    truncated to whole numbers, the concept of age is continuous) 
    o Education: no further information provided 
    

 Behavioral: 

    o Current Smoker: whether or not the patient is a current smoker (Nominal) 
    o Cigs Per Day: the number of cigarettes that the person smoked on average in 
    one day.(can be considered continuous as one can have any number of 
    cigarettes, even half a cigarette.) 

 Information on medical history: 

    o BP Meds: whether or not the patient was on blood pressure medication 
    (Nominal) 
    o Prevalent Stroke: whether or not the patient had previously had a stroke 
    (Nominal) 
    o Prevalent Hyp: whether or not the patient was hypertensive (Nominal) 
    o Diabetes: whether or not the patient had diabetes (Nominal) 

 Information on current medical condition: 
    
    o Tot Chol: total cholesterol level (Continuous) 
    o Sys BP: systolic blood pressure (Continuous) 
    o Dia BP: diastolic blood pressure (Continuous) 
    o BMI: Body Mass Index (Continuous) 
    o Heart Rate: heart rate (Continuous - In medical research, variables such as 
    heart rate though in fact discrete, yet are considered continuous because of 
    large number of possible values.)
    o Glucose: glucose level (Continuous)

 Target variable to predict:

    o 10 year risk of coronary heart disease (CHD) - (binary: “1”, means “Yes”, “0” 
    means “No”)
