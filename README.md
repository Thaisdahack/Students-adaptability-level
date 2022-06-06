# Students' Adaptability Level Prediction in Online Education using Machine Learning Approaches

Online Education has become increasingly popular since the COVID-19 has hit the world. Most educational institutions found online alternatives to continue educational activities, but many difficulties were encountered by students when introduced to this type of distance education. Considering this perspective, it is important that decision makers in educational institutions are informed about the effectiveness of online education so that they can take more measures to make it more profitable for students and that these courses have a high engagement and also generate value for the educational market 

<img src = "![EaDcapa](https://user-images.githubusercontent.com/101371267/169586956-8e426dc9-5b39-4079-8ce8-3b77f0e4e944.jpg)" width = "390">

## Goals

In this project, a dataset provided by Kaggle was used, where data collected through a survey carried out in Bangladesh shows the level of adaptability (low, high, moderate) of students to distance education between December 2020 and February 2021.
As a result, prediction models were applied to identify which of the 14 parameters evaluated in the survey would be most related to student engagement in online classes.
To get an idea of the effectiveness of online education and which main socioeconomics factors influence the adaptability of students, several machine learning algorithms were applied using Python's Pycaret library.

![fotosws](https://user-images.githubusercontent.com/101371267/171920621-78de3226-e144-4bbd-b506-8297052eebd0.png)

## To contextualize the subject globally, some relevant data on the e-learning market were collected:

USA, India, China, South Korea and the United Kingdom are the countries that invest the most in online education (Dos Santos, 2019);

The market size in 2021: 315 billion (USD);
Projected value for 2028: 1 trillion (USD);

![paises](https://user-images.githubusercontent.com/101371267/171921889-3d6dee3b-e19e-4669-8ca8-97f900fc7603.jpeg)

## Trends

## North America & Europe
Increased demand in the health care sector;
Increase in content digitization;
Moving from LMS to cloud-based systems;   
                                          
## West Asia & Latin America
Growth in higher education sectors;
Companies updating their training programs;
Growing demand for online English courses;

## Middle East & Africa
Government programs and initiatives on the rise;
Increasing diffusion of the internet and mobile learning;
source: gminsights

## Results

### Adaptability Level and Genres

Most respondents said they had moderate adaptability to distance education, followed by low adaptability and few people said they were highly comfortable with online learning  

![nivel adp](https://user-images.githubusercontent.com/101371267/171952948-87c57530-74fe-4d41-b07c-d87f6f24caf5.png)

When we talk about gender distinction, men are mostly at a moderate or high level of adaptability, while among women, few feel able to participate in online classes.

![adpXgenero](https://user-images.githubusercontent.com/101371267/171953291-d3ccaeae-0f58-4f22-90aa-21afeb68d20d.png)

### Socioeconomic Factors

Age: students with high or moderate adaptability are mostly aged between 11-15 years and 21-25 years 

![adpXidade](https://user-images.githubusercontent.com/101371267/171954647-998a072b-a890-4aed-ad6a-146faf406cc3.png)

The vast majority of students live in the city

![vivem na cidade](https://user-images.githubusercontent.com/101371267/171954820-426b8f34-e0d1-4829-96f2-cf91dd7417a9.png)

Financial condition does not seem to be a major impediment to participating in online courses, since average people in this regard seem to have moderate or high adaptability

![condiçao financeira](https://user-images.githubusercontent.com/101371267/171955378-a7b30c99-e763-483e-b03b-2fb16b38dc06.png)

### Other factors

The duration of classes between 1-3 hours is a significant parameter in student engagement in online courses 

![duraçao das aulas](https://user-images.githubusercontent.com/101371267/171955836-feb3bf1c-6895-4cd5-9f8f-02f88881b45f.png)

And the type of device most used for this activity is the mobile phone  

![tipo de dispositivo](https://user-images.githubusercontent.com/101371267/171955952-d9adefcc-e68e-47e0-afce-8fada8a7bdb8.png)

### Models

As there was a difference in the amount of responses between men and women, two models were made, one unbalanced with the original dataset and the other balanced by the SMOTE method.

## Original Dataset (unbalanced)
Target: adaptability level (low, moderate, high)

Best model: Extra Tree Classifier
Most important feature: Male gender/ Duration of classes
Accuracy: 0.88
AUC: 0.96
![Confusion Matrix_et](https://user-images.githubusercontent.com/101371267/171957420-841e9e2f-1970-4d0a-b328-1e5bde0e2140.png)

## Balanced Dataset
Target: adaptability level (low, moderate, high)

Best model: Random Forest
Most important feature: Average Financial Condition
Accuracy: 0.86
AUC: 0.96
![Confusion Matrix_rf](https://user-images.githubusercontent.com/101371267/171957641-a0af71e5-4e6d-449a-9f04-85a737cebd9b.png)

# Conclusions

Both models performed well, but it is interesting to observe which is the most significant parameter to be considered in each of them.
In general, the target audience for this type of market in Bangladesh is male with average financial conditions and also short courses that can be used on mobile phones.

## References

 - [Kaggle](https://www.kaggle.com/datasets/mdmahmudulhasansuzan/students-adaptability-level-in-online-education)

 - [Tableau Public](https://public.tableau.com/app/profile/thais.helena.dias/viz/Adaptabilityofstudentstoonlineeducation/Histria1?publish=yes)
