# Heart-Disease-Prediction
### Data:
[Data](https://www.kaggle.com/datasets/rashikrahmanpritom/heart-attack-analysis-prediction-dataset)
- Age : Age of the patient

- Sex : Sex of the patient

- exang: exercise induced angina (1 = yes; 0 = no)

- ca: number of major vessels (0-3)

- cp : Chest Pain type chest pain type
a)Value 1: typical angina
<br>b)Value 2: atypical angina
<br>c)Value 3: non-anginal pain
<br>d)Value 4: asymptomatic
- trtbps : resting blood pressure (in mm Hg)
- chol : cholestoral in mg/dl fetched via BMI sensor
- fbs : (fasting blood sugar > 120 mg/dl) (1 = true; 0 = false)
- rest_ecg : resting electrocardiographic results
a)Value 0: normal
<br>b)Value 1: having ST-T wave abnormality (T wave inversions and/or ST elevation or depression of > 0.05 mV)
<br>c)Value 2: showing probable or definite left ventricular hypertrophy by Estes' criteria
<br>d)thalach : maximum heart rate achieved
- target : 0= less chance of heart attack 1= more chance of heart attack

### EDA:
<p> First, we saw here the datatype of the parameters using data.info() then we checked the number of duplicate records in the dataset and then removed it.Then
  we also checked for the NULL values in the dataset using data.isnull() and then removed the NULL values.</p>
  
### Detecting Outliers:
Detecting Outliers using Seaborn's Boxplots:
<br> Here we found that outliers are present in trtbps, chol, thalachh, oldpeak, caa, thall.

## Removing Outliers:
1. Removing the outliers using IQR(Inter-Quartile Range):
In IQR the data points that are not in the range (lower limit, upper limit) are considered as outliers.
- upper limit = Q3 + 1.5 * IQR
- lower limit = Q1 – 1.5 * IQR
Afetr performing IQR, we found that 228 records still remain.

2. Removing outliers using Z-score:
- Here the data point is considered as an outlier if the corresponding Z-score > 3.
After performing Z-score we found that 287 records still remain.

As after performing Z-score we have more number of records, we preferred Z-score.

## Correlation:
1. Finding Correlation using Seaborn's Heatmap:
<p align="center">
<img src="https://github.com/prathammehta16/Heart-Disease-Prediction/blob/images/sns.png">
</p>
2. Finding Correlation using Pearson's Correlation:
<p align="center">
<img src="https://github.com/prathammehta16/Heart-Disease-Prediction/blob/images/pearson.png">
</p>
3. Finding correlation using Spearman's correlation:
<p align="center">
<img src="https://github.com/prathammehta16/Heart-Disease-Prediction/blob/images/spearman.png">
</p>

## Training Models:
Here the models we used to predict are:
1.Logistic Regression
2.Decision Trees
3.Random Forest
4.K nearest neighbor.
<br> And their corresponding accuracy scores are:
<p align="center">
<img src="https://github.com/prathammehta16/Heart-Disease-Prediction/blob/images/output.png">
</p>
