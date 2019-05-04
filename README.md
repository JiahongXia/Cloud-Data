# Cloud-Data
Stat 154 spring 2019 project 2

Part 1(Run the proper method)
We first developed two different methods to split the data, and we put different methods in
different cells. You need to make sure you run the method cells correctly before you continue to the next part. 

Part 2(Just run the cell)
Then we generic cross-validation (CV) function CVgeneric in R that takes a generic classifier, training features, training labels, number of folds K and a loss function as inputs and outputs the K-fold CV loss on the training set.
The cutoff values, whose default value is 0.5 in the function, is given by the user, the function couldn't optimize this argument. CVgeneric returns a list of K elements, each element contains the confusion matrix, overall accuracy, etc,  of each fold. 

Part 3 (Can change the cutoff value)
Then we tried "glm","lda","qda","svm" into the CVgeneric function, and get split_method_2.csv as a result. (When choosing method 1, you should change the output name in order to prevent the CSV file from recovering. Then you can just run the 3(b) cell directly, and the cutoff value we highlight in this part is 0.5.

Part 4 (Just run the cell)
We made an in-depth analysis of a "qda" classification model. We used the function partimat in package “klaR”, partimat provides a multiple figure array which shows the classification of observations based on classification methods for every combination of two variables. Based on our analysis, we chose to use the Random Forest Algorithm.


