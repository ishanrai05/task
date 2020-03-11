# Machine Learning Part

## Task
You will explore how best to apply machine learning algorithms, for example, Neural Network, Boosted Decision Tree (BDT), Support Vector Machine(SVM) to solve a High Energy Data analysis issue, more specifically,  separating the signal events from the background events.
A set of input samples (simulated with Delphes) is provided in NumPy NPZ format [Download Input]. In the input file, there are only 100 samples for training and 100 samples for testing so it won’t take much computing resources to accomplish this task. The signal events are labeled with 1 while the background sample are labeled with 0.
You can apply one machine learning algorithm to this input but be sure to show that you understand how to fine tune your machine learning model to improve the performance. The performance can be evaluated with classification accuracy or Area Under ROC Curve (AUC).

## Analysis

I have done detailed visualization and analysis of the dataset and applied various models in the dataset.

I have also trained various models for the task of prediction but none of them have produced any satisfactory results, probably because of very few dataset for training. I have plotted ROC-AUC curve and found out the accuracy, precision and recall as well plotted the accuracy matrix for all the models, which is present in the notebook.

## Data Visualization and Exploratory Data Analysis


### Basetrack distributions for background for each column in dataset

![Signal](../images/0_1.png)
<img src="../images/0_5.png" max_width=400px/>



### Basetrack distribution for signals for each column in dataset

![Background](../images/1_0.png)
<img src="../images/1_4.png" max_width=400px/>

### 3D visualization for all combinations of components in dataset

![1](../images/012.png)
![2](../images/013.png)
![3](../images/014.png)
![4](../images/023.png)
![5](../images/024.png)
![6](../images/034.png)
![7](../images/123.png)
![8](../images/124.png)
![9](../images/134.png)
![10](../images/234.png)

## Models Used and description

### DNN 

![loss](../images/dnn_model_loss.png)
![accuracy](../images/dnn_model_accuracy.png)
![roc](../images/dnn_roc_auc.png)
![cf](../images/dnn_cf_matrix.png)

### XGBClassifier

![roc](../images/xgb_roc_auc.png)
![cf](../images/xgb_cf_matrix.png)

### AdaBoostClassifier

![roc](../images/ada_roc_auc.png)
![cf](../images/ada_cf_matrox.png)

### GradientBoostingClassifier

![roc](../images/gb_roc_auc.png)
![cf](../images/gb_cf_matrix.png)

### Support Vector Machine

![cf](../images/svm_cf_matrix.png)

### KNeighborsClassifier

![cf](../images/knn_cf_matrix.png)

### LogisticRegression

![cf](../images/lr_cf_matrix.png)

### DecisionTreeClassifier

![cf](../images/dt_cf_matrix.png)

### RandomForestClassifier

![cf](../images/rf_cf_matrix.png)
