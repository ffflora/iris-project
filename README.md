The goal of this project is to get used to the Scikit-learn SVM API. I also add XGBoost algorithm ( booster: `gblinear` ) for comparison.  

Dataset:

[Iris Dataset.](https://en.wikipedia.org/wiki/Iris_flower_data_set)

This project shows the difference of the decision surfaces for difference kernels. 

Comparison of different linear SVM classifiers on a 2D projection of the iris dataset. We only consider the first 2 features of this dataset:

- Sepal length
- Sepal width 

The accuracy of the chosen algorithms are as follows:

```
0.8 			# 'SVC with linear kernel',
0.6888888888888889	# 'LinearSVC (linear kernel)',        
0.7777777777777778	# 'SVC with RBF kernel',
0.7777777777777778	# 'SVC with polynomial (degree 3) kernel',
0.5111111111111111	# 'xgboost with gblinear'
```

![](https://raw.githubusercontent.com/FFFlora/iris-project/master/plot.png)

---
In this part I added ROC-AUC curve with 6-fold cross valication, and calculated the AUC (area under the curve) of iris dataset. The figure roughly shows how the classifier output is affected by changes in the training data.

![](https://raw.githubusercontent.com/FFFlora/iris-project/master/ROC-AUC_curve.png)
