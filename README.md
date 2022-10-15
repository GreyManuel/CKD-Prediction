## Author:
## Grey Manuel
# Chronic Kidney Disease Prediction
This is a machine learning project that is trained on collected data of sample xray images of kidneys with CKD.
<br/>
It includes a lot of data about the individual images used for training and I used that feature to make an optimal model that will predict if a kidney is healthy or not
<br/><br/>
## Solution approach in this model
### Data preparation part
- The dataset has very low data records but a little bit better amount of features/columns. So, I added more columns by combining existing one to get many number of columns to work with. Since, we don't have enough data, that was my only option.
- The dataset has some columns with a lot of null values. I removed these columns since they will surely bias my model if I was to impute them.
- I removed some rows which have at least one null record. Because, they will corrupt the model.
<br/>

### Model training part
- I used accuracy, precision, recall and F1 scores as model measuring metrices.
- I tried support vector machine, decision tree and random forest algorithms.
- Support vector machine was severly overfitting the dataset
- Decision tree was not fitting in quite as good as random forest. Because, the accuracy and other metrics were very low relatively to the random forest. Since, random forest is collection of decision trees, that will cover the issue of a single decision tree algorithm.
- RandomForest was fitting in the dataset quite very well. Ofcourse there is a little bit of over fitting but better than support vector machine. So, my final model is Random forest algorithm.
<br/>
<p align="center">
  <img src="imgs\rec.png" width="700" >
</p>
