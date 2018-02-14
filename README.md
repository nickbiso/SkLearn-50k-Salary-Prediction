# >50k Salary Prediction
Dataset is acquired from the following link: https://archive.ics.uci.edu/ml/datasets/adult

# Dataset Summary:
## Data is Unbalanced 3:1
![alt text](https://github.com/nickbiso/50k-Salary-Prediction/blob/master/plots/unbalanced.png)

## Age is a key factor
![alt text](https://github.com/nickbiso/50k-Salary-Prediction/blob/master/plots/age.png)

## Individuals who make money by investing usually earn more  
![alt text](https://github.com/nickbiso/50k-Salary-Prediction/blob/master/plots/capitalgains.png)

## Indivuduals who have higher education earn more money
![alt text](https://github.com/nickbiso/50k-Salary-Prediction/blob/master/plots/education.png)

# Machine Learning Results
## Accuracy


|Machine Learning Algorith      |	Imbalanced |	Undersampling (Balanced)	|	 Oversampling (Balanced)	  |
|:----------------------|:-------------------:|:-------------:|:---------------:|
|	Support Vector Machine|	33%	                |	40%	          |	**42%**	            |
|	K-Nearest Neighbor	  |	**64%**	                |	60%	          |	62%	            |
|	Random Forest	        |	**65%**	                |	69%	          |	69%	            |           
|	Gradient Boosting	    |	**69%**	                |	70%	          |	70%	            |
|	Extra Trees	          |	**44%**               	|	65%	          |	68%	            |
|	Neural Network	      |	**40%**	                |	43%	          |	41%	            |
|	Adaboost	            |	**61%**               	|	64%	          |	67%	            |
|	Decision Tree	        |	**60%**                |	63%         	|	62%	            |

