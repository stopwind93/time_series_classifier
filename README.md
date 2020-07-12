# Time Series Data Classifier
3 datasets (ToolA, ToolB, ToolC), each containing time series sensor data from a different manufacturing tool (A, B, C). 
The objective is to build a model to determine any given time series sample is from which tool. 

## Steps
### 1) Import Libraries
- os
- numpy
- pandas
- pickle
- matplotlib
- sklearn

### 2) Load, Summarize and Visualize Dataset
Time series = 1 --> 400  
Total dataset per Tool = 100  
Total Tool = 3  

### 3) Separate Dataset & Train Models
Separate datasets to 70/30.  
70% of the data will be used to train. 30% of the data will be used to validate.  
Total 6 models are being used to train:  
- Logistic Regression
- K-Nearest Neighbours Clasifier
- Decision Tree Classifier
- Support Vector Machines
- Random Forest Classifier
- Gradient Boosting Classifier

### 4) Evaluate Further using Cross Validation
- LR Accuracy: 0.98 (+/- 0.04) 	Time Taken: 1.45 sec  
- KNN Accuracy: 1.00 (+/- 0.00) 	Time Taken: 0.55 sec  
- CART Accuracy: 1.00 (+/- 0.00) 	Time Taken: 0.39 sec  
- SVM Accuracy: 0.98 (+/- 0.05) 	Time Taken: 0.28 sec  
- RF Accuracy: 1.00 (+/- 0.00) 	Time Taken: 0.64 sec  
- GBM Accuracy: 0.99 (+/- 0.02) 	Time Taken: 6.60 sec  

## Conclusion
It can be observed only KNN, Cart and RF have an accuracy of 100% without any std dev.  
CART takes the least time to complete as compared to KNN and RF. CART would be the best model for this task.  
