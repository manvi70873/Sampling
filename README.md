# Sampling
Assignment on Sampling for UCS654

## Description
This assignment has a dataset regarding credit cards.
It is a binary classification problem.
The dataset is imbalanced and hence it is balanced by using random over sampling technique.
After balancing the dataset, different sampling techniques are used and 5 different models have been applied to get the accuracy on testing set.
The dataset is divided into a 25-75 ratio of testing and training set.

## Methodology
1. Balancing Dataset
2. Creating different types of samples
3. Training different machine learning models
4. Testing the models
5. Analysing the Result obtained

## Sampling Technique Description and Sampling Size Formula
1.RandomUnderSampler:-The RandomUnderSampler algorithm works by randomly selecting a subset of the majority class instances that are equal to the number of minority class instances. This results in a balanced dataset with equal proportions of each class.
2.RandomOverSampler:-The RandomOverSampler algorithm works by randomly selecting a subset of the minority class instances and duplicating them until the number of minority class instances is equal to the number of majority class instances.
3.SMOTE:-The SMOTE algorithm works by creating synthetic examples of the minority class by interpolating between existing minority class instances.
4.TomekLinks:-The TomekLinks algorithm works by identifying all pairs of samples that are nearest neighbors and belong to different classes. Among these pairs, it identifies those pairs where removing the majority class sample would increase the distance between the two classes.
5.NearMiss:-The NearMiss algorithm works by selecting the nearest neighbors of the minority class instances in the feature space. There are three variants of the NearMiss algorithm: NearMiss-1, NearMiss-2, and NearMiss-3.

## Final Result Table
|                        | RandomUnder   | RandomOver | SMOTE      | TomekLinks| NearMiss    |
| ---------------------- | ------------- | ---------- | ---------- | -------   | ----------- |
| Logistic Regression    |0.5742         |0.9935      |0.9935      |0.9935     |0.3742       |
| Decision Tree          |0.5742         |0.9806      |0.9806      |0.9806     |0.6968       |
| RandomForestClassifier |0.7097         |0.9935      |0.9935      |0.9935     |0.7677       |
| SVC                    |0.6258         |0.9935      |0.9935      |0.9935     |0.5161       |
| ExtraTrees	           |0.8065         |0.9935      |0.9935      |0.9935     |0.6516       |

## Discussion
From the table, we can conclude that we achieve maximum accuracy when we apply RandomForestClassifier.


## License
[MIT](https://choosealicense.com/licenses/mit/)


