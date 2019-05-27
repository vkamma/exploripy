# ExploriPy
Pre-Modelling Analysis of the data, by doing various exploratory data analysis and Statistical Test.

**Installation Steps**

``` pip install ExploriPy ``` 

**Important Parameters**
* data : Complete Dataset, should be a Pandas DataFrame. 
* CategoricalFeatures : List of Categorical Features
* title : Title which should appear in the top of the HTML file

**Installation Steps**

```
from ExploriPy import EDA
df = pd.read_csv('LoanPrediction.csv',na_values = 'nan')
CategoricalFeatures = ['Gender', 'Married', 'Dependents', 'Education', 'Self_Employed', 'Credit_History',
                                 'Property_Area', 'Loan_Status', 'Loan_Amount_Term']
eda = EDA(df,CategoricalFeatures,title='Data Analysis on a Public Data')
eda.EDAToHTML()
```

**Output**


<p>
<img src='/ExploriPy/doc_images/Null.PNG'></img>


<p>
<img src='/ExploriPy/doc_images/Continuous.png'></img>


<p>
<img src='/ExploriPy/doc_images/Correlation Heatmap.PNG'></img>
  

<p>
<img src='/ExploriPy/doc_images/Scatter Plot.PNG'></img>


<p>
<img src='/ExploriPy/doc_images/Feature Reduction.PNG'></img>


<p>
<img src='/ExploriPy/doc_images/Categorical.PNG'></img>
  
**Categorical Vs Categorical**
<p>
Weight Of Evidence, Information Value, Chi-Sq Test of Independence
<img src='/ExploriPy/doc_images/WOE IV ChiSq.png'></img>

**Categorical Vs Continuous**
<p>
ANOVA and PostHoc Test (Tukey HSD)
<img src='/ExploriPy/doc_images/Anova TukeyHSD.png'></img>
