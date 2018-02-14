# >50k Salary Prediction
Dataset is acquired from the following link: https://archive.ics.uci.edu/ml/datasets/adult

# Dataset Summary:

This Dataset has 32561 observations. 

## Data is Unbalanced 3:1
![alt text](https://github.com/nickbiso/50k-Salary-Prediction/blob/master/plots/unbalanced.png)

## Age is a key factor
![alt text](https://github.com/nickbiso/50k-Salary-Prediction/blob/master/plots/age.png)

## Individuals who make money by investing usually earn more  
![alt text](https://github.com/nickbiso/50k-Salary-Prediction/blob/master/plots/capitalgains.png)

## Indivuduals who have higher education earn more money
![alt text](https://github.com/nickbiso/50k-Salary-Prediction/blob/master/plots/education.png)

# Machine Learning Results 
For this exercise I utilized different machine learning algorithms that are available on sklearn. I used these algorithms on the different sampling methods of the original dataset to balance it.

## f1-score
Different algorithms reacted to sampling methods differently. The over-arching theme here is that balancing the dataset increases the f1-score.

|Machine Learning Algorithm      |	Imbalanced |	Undersampling (Balanced)	|	 Oversampling (Balanced)	  |
|:----------------------|:-------------------:|:-------------:|:---------------:|
|	Support Vector Machine|	33%	                |	40%	          |	**42%**	            |
|	K-Nearest Neighbor	  |	**64%**	                |	60%	          |	62%	            |
|	Random Forest	        |	65%	                |	**69%**	          |	69%	            |           
|	Gradient Boosting	    |	69%	                |	**70%**	          |	70%	            |
|	Extra Trees	          |	44%               	|	65%	          |	**68%**	            |
|	Neural Network	      |	40%	                |	**43%**	          |	41%	            |
|	Adaboost	            |	61%               	|	64%	          |	**67%**	            |
|	Decision Tree	        |	60%                |	**63%**         	|	62%	            |

## Accuracy(Test Set)
Despite increasing the f1-score, balancing the dataset did not perform as well in terms of the accuracy. This can be attributed to the fact that the distribution of the train set and the test set becomes different. 

|Machine Learning Algorithm      |	Imbalanced |	Undersampling (Balanced)	|	 Oversampling (Balanced)	  |
|	:---	|	:---:	|	:---:	|	:---:	
|	Support Vector Machine	|	79%	|	25%	|	**79%**	|
|	K-Nearest Neighbor	|	**83%**	|	74%	|	75%	|
|	Random Forest	|	**85%**	|	80%	|	81%	|
|	Gradient Boosting	|	**86%**	|	81%	|	81%	|
|	Extra Trees	|	**82%**	|	75%	|	81%	|
|	Neural Network	|	**80%**	|	79%	|	78%	|
|	Adaboost	|	**84%**	|	75%	|	79%	|
|	Decision Tree	|	**81%**	|	79%	|	76%	|
