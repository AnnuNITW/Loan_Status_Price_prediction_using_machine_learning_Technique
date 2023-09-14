# Loan-Status-Prediction-using-Support-Vector-Machine

Hello Everyone, I hope you are doing well. Ever wondered, how great would it be, if we could predict, whether our request for a loan, will be approved or not, simply by the use of machine learning, from the ease and comfort of your home? 
I am doing that with the help of a Machine Learning model named the Support Vector Machine.

<img src ="https://user-images.githubusercontent.com/108235140/203006550-66b17bc6-8dd6-4b98-a1a3-36456efa16c8.png">

## A brief about Support Vector Machine Model

The algorithm that I am using for this purpose, is the Support Vector Machine. Support Vector Machine,(SVM), falls under the “supervised machine learning algorithms” category. It can be used for classification, as well as for regression. In this model, I plot each data item as a unique point in an n-dimension,(where n is actually, the number of features that we have), with the value of each of the features being the value of that particular coordinate. Then, I perform the process of classification by finding the hyper-plane that differentiates the two classes.

## Why choose Support Vector Machine over other algorithms?

It all depends on the type of operations we are performing, and the type of data we are dealing with. SVM is preferred over other algorithms when :
- The data is not regularly distributed.
- SVM is generally known to not suffer the condition of overfitting.
- Performance of SVM, and its generalization is better on the dataset.
- And, lastly, SVM is known to have the best results for classification types of problems.

![image](https://user-images.githubusercontent.com/108235140/203007501-95bd2f23-0c4f-4daa-be8a-7960b675c2a8.png)
 
 ## Steps Involved
 
 ### Dataset
 
The foremost thing that is needed the most, in a machine learning project, is a dataset.
A dataset, as the name says, is a set or collection of data. It contains all the values that we need to work with, to get the necessary results.
For this project, the dataset that I have used is the one I found on Kaggle. You can use any dataset available on the internet that you feel comfortable working with.

### Importing Dependencies : 
The dependencies that we will be using are :
numpy, pandas, seaborn, and ScikitLearn.

### Data Collection and Processing

![image](https://user-images.githubusercontent.com/108235140/203012007-cb22d5e5-af49-479d-bff0-28653c3c8c6b.png)

- The dataset will be in the format of a CSV. Thus to read it, I am taking the help of the pandas method, called read_csv()
- Also I am storing the dataset in the variable called “loan_dataset” to refer to the entire dataset by this variable name.
- Now, I have checked the number of rows and columns in the dataset.
- After that I have checked, how many values are missing from the dataset.
- Furthur, I have deal with missing values and remove that anomaly using various methods.
- Now, After that, I have performed Label Encoding. I am replacing the loan status of ‘Y’ with 1, and ‘N’ with 0, for better reference.
- Then I have count the frequency of each value in the “Dependent” column. Replace the value of 3+ with 4 to better performance.
- Again, I convert the categorical columns, to numerical values for better reference.
- And lastly in this step, split the data and label into the X and Y variables : X will store all the features on which the loan status depends, excluding the loan status itself. Y will store only the Loan Statuses.

### Splitting X and Y into Training and Testing Variables

Here, I am splitting the data into four variables, viz., X_train, Y_train, X_test, Y_test. The testsize represents the ratio of how the data is distributed among X_trai and X_test (Here 0.2 means that the data will be segregated in the X_train and X_test variables in an 80:20 ratio). You can use any value you want. A value < 0.3 is preferred.

### Training our Support Vector Machine model

![image](https://user-images.githubusercontent.com/108235140/203011519-8a34f823-657b-4da4-8e20-0934c9bc7111.png)

Finally, I have trained my model and obtained the Accuracy of **79% on training dataset** and **83% on testing dataset**.

#### Conclusion: Since the Accuracy is very good, This model is now able to handle new input values and predict the output. Hope, this project will help you a lot :)

