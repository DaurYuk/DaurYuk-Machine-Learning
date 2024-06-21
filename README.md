<div align="center">
  <img src="https://drive.google.com/uc?export=view&id=1FAluquVilJW5e8XKUtnQt-D1YsBr4DxE" alt="DaurYuk Logo"></img>
  <h2 align="center">DaurYuk: Sorting Waste for a Sustainable Future!</h2>
</div>

## About the Dataset

In this project, we combined 2 different datasets to address the overfitting of the data. Those are:

**1. RealWaste Image Classification**
source: https://www.kaggle.com/datasets/joebeachcapital/realwaste/data

- 9 classes
- main dataset

**2. Garbage Classification**
source: https://www.kaggle.com/datasets/mostafaabla/garbage-classification/data

- 12 classes
- additional dataset

**Combined dataset (zip file) can be accessed through this link**
https://drive.google.com/file/d/1UZxOdmBwnuSxE93Arhm8La0WKKqodS28/view?usp=sharing

## About the Model

The model is made to classify waste object into eight different classes:

1. Cardboard
2. Food organics
3. Glass
4. Metal
5. Miscellaneous trash
6. Paper
7. Plastic
8. Textile trash

We use MobileNetV2, which has been trained on ImageNet, as the base model. In an effort to improve the accuracy, we also retrain the last half layers of the base model and add more layers in addition to the base model.

<details> 
  <summary> Image below is the final architecture of our model: </summary>
  <img src="https://drive.google.com/uc?id=1XyuCsJ7wrk_yuI9hjEy6m4ACTnGV3byA" alt="Model architecture"></img>
</details>
<br>

With this model, we manage to achieve 92% testing accuracy with details below.

```Text
                     precision    recall  f1-score   support

          Cardboard       0.89      0.95      0.92       275
      Food Organics       0.95      0.99      0.97       377
              Glass       0.93      0.96      0.94       491
              Metal       0.93      0.85      0.88       308
Miscellaneous Trash       0.95      0.85      0.90       274
              Paper       0.92      0.91      0.91       321
            Plastic       0.86      0.89      0.87       343
      Textile Trash       0.97      0.96      0.97       365

           accuracy                           0.92      2754
          macro avg       0.92      0.92      0.92      2754
       weighted avg       0.92      0.92      0.92      2754
```

This confusion matrix provides a clear picture of how well the model performs on a test dataset, going beyond simple accuracy.
<img src="https://drive.google.com/uc?id=11jvDdlU5rktOK6gi03eKRkFiLZ6ejW_r" alt="Confusion matrix of testing result"></img>
