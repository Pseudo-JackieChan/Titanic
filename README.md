# Titanic Dataset (Seaborn)

This repository provides documentation and examples for the **Titanic dataset** available in the [Seaborn library](https://seaborn.pydata.org/).  
The dataset contains demographic and survival information for passengers aboard the Titanic.

---

## 📊 Dataset Overview

The Titanic dataset is a classic resource for practicing data analysis, visualization, and machine learning.  
It includes variables such as passenger class, sex, age, fare, and survival status.

### Features

| Column       | Description                                                                 |
|--------------|-----------------------------------------------------------------------------|
| `survived`   | Survival indicator (0 = No, 1 = Yes)                                        |
| `pclass`     | Passenger class (1 = First, 2 = Second, 3 = Third)                          |
| `sex`        | Gender of the passenger                                                     |
| `age`        | Age in years                                                                |
| `sibsp`      | Number of siblings/spouses aboard                                           |
| `parch`      | Number of parents/children aboard                                           |
| `fare`       | Ticket fare                                                                 |
| `embarked`   | Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)        |
| `class`      | Passenger class (string equivalent of `pclass`)                             |
| `who`        | Passenger type (man, woman, child)                                          |
| `adult_male` | Boolean indicator for adult male                                            |
| `deck`       | Deck level (where available)                                                |
| `embark_town`| Town of embarkation                                                         |
| `alive`      | Survival status (string equivalent of `survived`)                           |
| `alone`      | Boolean indicator if passenger was traveling alone                          |

---

## 📦 Loading the Dataset

You can load the dataset directly using Seaborn:

```python
import seaborn as sns

# Load Titanic dataset
titanic = sns.load_dataset("titanic")

# Preview the first few rows
print(titanic.head())
