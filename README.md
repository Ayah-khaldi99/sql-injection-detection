# sql-injection-detection
using hybrid Dl-ML model on sql injection detection.
In our resaerch we used a hybrid approach that combines the capabilities of pre-trained RoBERTa and BERT deep learning models for featuer extraction with traditional machine learning (ML) algorithms SVM , RF, DT, and logistic regression.

![sql-injection-hybrid-model-arch](https://github.com/Ayah-khaldi99/sql-injection-detection/assets/112800075/d9635875-046f-4985-a324-85fa70e40ba2)


## Dataset:
#### Data set cleaining:
Under `dataset-preprocessing` file you will see the steps of data set cleaining starting from collecting data from several Kaggle dataets until split the cleaned dataset to 3 sets (train, test, val) by 6:2:2 and then split the training dataset to 4 training sets (to use them on the 4 ML models).
###### Dataset Kaggle link: https://www.kaggle.com/datasets/ayahkhaldi/sql-injection-dataset 
###### Dataset was cleaned by these Kaggle datasets:
- https://www.kaggle.com/datasets/syedsaqlainhussain/sql-injection-dataset/data
- https://www.kaggle.com/datasets/sajid576/sql-injection-dataset
- https://www.kaggle.com/datasets/gambleryu/biggest-sql-injection-dataset
- https://www.kaggle.com/datasets/mahdighaemi/sql-injection
- https://www.kaggle.com/datasets/kholoodsalah/sql-injection-dataset
- https://www.kaggle.com/datasets/alextrinity/sqlinjectionextend

#### Data set folder:
In this folder you can see **three sets (train, test, val)** which are the result of our data preprocessing, and **four train sets** that were split from the `Train.csv` dataset to use them in our four ML models.
![sql-injection-datasets](https://github.com/Ayah-khaldi99/sql-injection-detection/assets/112800075/4970d91e-0ebd-42d1-8f60-b44ad161e860)
![train-sets](https://github.com/Ayah-khaldi99/sql-injection-detection/assets/112800075/709e22c7-e9cb-4a88-ad7b-404741d052f9)


## Models:
we used each of RoBERTa and BERT with SVM , RF, DT, and logistic regression models you can see the usage under `sql-injection-hybrid-model.ipynb` file with its result.

![results](https://github.com/Ayah-khaldi99/sql-injection-detection/assets/112800075/71fcb0d0-a64a-415e-84d2-ae123bf5868f)


## Predections:
In the folder predictions you will see all predctions per model on `predections-per-model` file, and the final voting result in the `voting-ensemble-predictions` file.
