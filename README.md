# Heart-Disease-Prediction
### Data:
[Data](https://www.kaggle.com/datasets/rashikrahmanpritom/heart-attack-analysis-prediction-dataset)
- Age : Age of the patient

- Sex : Sex of the patient

- exang: exercise induced angina (1 = yes; 0 = no)

- ca: number of major vessels (0-3)

- cp : Chest Pain type chest pain type

<br>a)Value 1: typical angina
<br>b)Value 2: atypical angina
<br>c)Value 3: non-anginal pain
<br>d)Value 4: asymptomatic
<br>- trtbps : resting blood pressure (in mm Hg)

- chol : cholestoral in mg/dl fetched via BMI sensor

- fbs : (fasting blood sugar > 120 mg/dl) (1 = true; 0 = false)

- rest_ecg : resting electrocardiographic results

<br>a)Value 0: normal
<br>b)Value 1: having ST-T wave abnormality (T wave inversions and/or ST elevation or depression of > 0.05 mV)
<br>c)Value 2: showing probable or definite left ventricular hypertrophy by Estes' criteria
<br>d)thalach : maximum heart rate achieved

<br>- target : 0= less chance of heart attack 1= more chance of heart attack

### EDA:
<p> First, we saw here the datatype of the parameters using data.info() then we checked the number of duplicate records in the dataset and then removed it.Then
  we also checked for the NULL values in the dataset using data.isnull() and then removed the NULL values.</p>

