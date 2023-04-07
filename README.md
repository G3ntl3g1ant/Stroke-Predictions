# Stroke Predictions
#### A Dataset of Patients Information with General Information and whether they have had a Stroke or Not.
### Author: Kai Dawson-Fischer
## Question: 
#### Can physicians predict who will be a stroke victim before one even occurs?

## Data 
#### Data Source:
https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset

#### Data Dictionary:


![Stroke Predictions Data Dictionary](https://user-images.githubusercontent.com/117219099/230604916-966c98ec-bc5a-48ce-b765-d36c5d8c1da6.png)

## Methods
- Processed the data by removing duplicates
- Dropped the 'id' column due to that it was too unique a value
- Dropped the 'gender' value of 'other' and 'work_type' value of 'Never_worked' due to that they made up less than 5% the DataFrame, deeming them unnecessary.
- Changed the values of 'gender', 'ever_married', and the 'Residence_type' columns into numerical values due to that they were binary in nature, leading to changing their column titles to 'is_female', 'ever_married'(this one remained the same), and 'is_urban', respectively. 
## Results
![Scatterplot of Glucose Level and BMI](https://github.com/G3ntl3g1ant/Stroke-Predictions/blob/main/Scatterplot%20of%20Glucose%20Level%20and%20BMI.png)

Here it is facinating to see how the data flow seems to move like an hourglass for BMI and Glucose Level, with assuming that the glucose levels are after fasting, most are on the lower end of pre-diabetic if not even diabetic. Then, thinning out and then expanding, leading into diabetic status seeming as though that those on the border of diabetes concentrate closer on the BMI range of 30 or higher, which by the standards of the CDC is the range of obesity. 

(Resource: https://www.cdc.gov/healthyweight/assessing/index.html#:~:text=If%20your%20BMI%20is%20less,falls%20within%20the%20obese%20range.)

![Scatterplot of Glucose Level and BMI with Stroke](https://github.com/G3ntl3g1ant/Stroke-Predictions/blob/main/Scatterplot%20of%20Glucose%20Level%20and%20BMI%20with%20Stroke.png)

With this scatterplot we can see that Strokes seem to occur rarely and accross the board for all BMI numbers and Glucose Levels. 

![BMI Vs Age: Focus on Marriage Status](https://github.com/G3ntl3g1ant/Stroke-Predictions/blob/main/BMI%20Vs%20Age%20Focus%20on%20Marriage%20Status.png)

When it comes to this plot it is intriguing to see the slight arch over the data as far as BMI over time, showing that most 
gain weight as they age, some more than others. But it is also interesting to see the number of people that seem to start getting married around their 30s and then increasing throughout the data(of course with the peppered outliers). 

![BMI Vs Age: Focus on Stroke Occurrence](https://github.com/G3ntl3g1ant/Stroke-Predictions/blob/main/BMI%20Vs%20Age%20Focus%20on%20Stroke%20Occurrence.png)

We can see here that even with the varying BMIs, the Ages are what truly show a difference. Strokes do not start making an appearance until around the age of 45. 

## Model
The final model that was chosen was the KNeighbors Model

              precision    recall  f1-score   support

           0       0.95      0.86      0.90      1192
           1       0.15      0.38      0.21        80

    accuracy                           0.83      1272


With the scores of 0.38 for recall and 0.21 for f1-score, this was the best model by far. 

With the next closest model only able to achieve 0.07 for recall and 0.11 for the f1-score.

## Reccomendations
To speak franky, this model would have a partial likelihood of predicting a stroke, but there needs to be more data to be able to achieve a better model. As of now the best choice is to eat right, exercise and regular visits to your General Practitioner Physician. 
## Limitations & Next Steps
This particular dataset is not normalized, there needs to be more data gathered in order for a viable model to be created. There needs to be more research on the particular stroke patients. The more cases of stroke patients available, the better a model can predict future victims. 
#### For further information:
For any additional questions, please contact kaidawsonfischer2022@gmail.com
