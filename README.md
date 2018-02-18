Exploratory Data Analysis of **Haberman's Survival Data Set :**

###### Overview
The dataset contains cases from a study that was conducted between 1958 and 1970 at the University of Chicago's Billings Hospital on the survival of patients who had undergone surgery for breast cancer.

| Data Source | Language | Libraries used | ipython notebook | .pdf report |
|-------------|----------|----------------|------------------|-------------|
| [Kaggle](https://www.kaggle.com/gilsousa/habermans-survival-data-set) | Python | pandas, matplotlib, seaborn | [Haberman.ipynb](https://github.com/rdrsadhu/habermans-cancer-survival-dataset/blob/master/Haberman.ipynb) | [Haberman.pdf](https://github.com/rdrsadhu/habermans-cancer-survival-dataset/blob/master/Haberman.pdf) |


###### Result
A pseudo-model which,

Given a new patient's (age, year-of-operation, count-of-positive-nodes-detected), predicts if the patient will survive for more than 5 years after the operation or not.

```Python

def predict(age, opyr, node):

    '''This function returns
        True: if a patient will survive for more than 5 years
        False: otherwise
    '''

    if age<=40:
        return True  # 90% success rate
    else:
        if node<=3:
            return True  # 80% success rate
        else:
            return
            # I need some help here
            # and would love to know how you would have analyzed this
```
