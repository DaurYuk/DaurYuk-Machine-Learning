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

We use MobileNetV2, which has been trained on ImageNet, as the base model. In an effort to improve the accuracy, we also retrain the last half layers of the base model.

Image below is the final architecture of our model:
<img src="https://drive.google.com/uc?id=1XyuCsJ7wrk_yuI9hjEy6m4ACTnGV3byA" alt="Model architecture"></img>
