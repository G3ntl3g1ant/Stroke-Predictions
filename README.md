# Stroke Predictions
#### A Dataset of Patients Information with General Information and whether they have had a Stroke or Not.
### Author: Kai Dawson-Fischer
## Question: 
#### Can strokes victims predict that they are going to suffer from a stroke before it even occurs?

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

Here it is facinating to see how the flow seems to move like an hourglass for BMI and Glucose Level, with assuming that the glucose levels are after fasting, most are on the lower end of pre-diabetic

![BMI Vs Age: Focus on Marriage Status](https://github.com/G3ntl3g1ant/Stroke-Predictions/blob/main/BMI%20Vs%20Age%20Focus%20on%20Marriage%20Status.png)

Text

![BMI Vs Age: Focus on Stroke Occurrence](https://github.com/G3ntl3g1ant/Stroke-Predictions/blob/main/BMI%20Vs%20Age%20Focus%20on%20Stroke%20Occurrence.png)

Text
## Model

## Reccomendations

## Limitations & Next Steps

#### For further information:
For any additional questions, please contact kaidawsonfischer2022@gmail.com
