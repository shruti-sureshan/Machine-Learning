# Machine-Learning

**1. Halfspace classifier and Logistic regression** <br/>
Choose an appropriate dataset of your choice such that every record (example) has at least 5 features which are numeric in nature and there is at least one attribute (feature) which is binary in nature. You can use the binary attribute as the binary target label to be predicted. In case you want to use a target variable which has more than two distinct values, then you can map them into two sets and give label 1 to one of the sets and 0 to the other. Thus, a multiclass classification task can be reduced to binary classification task. plit your dataset into a training set and a test set. You can try different splits: 70:30 (70% training, 30% testing), 80:20 or 90:10 split.
On the training set, train the following classifiers:
- Half Space classifier implemented using LP solver (one such solver is scipy.optimize.linprog)
- Half Space classifier implemented using Perceptron Algorithm (implement the iterations)
- Logistic Regression Classifier  (with Gradient descent for optimization)

**2. Linear Regression**<br/>
Select an appropriate dataset, select the independent features (input features) and the dependent feature (target feature), perform dataset split and train a linear regression classifier. Solve for the parameters of the machine using the following:
- Peudo-Iverse method 
- Gradient descent to minimize the squared error loss


**3. Support Vector Machine**<br/>
Use a dataset of your  choice and implement the following:
- Hard SVM learning rule by solving a Quadratic Program using the convex optimization package cvxopt_solvers.qp
- Soft SVM learning rule using  cvxopt_solvers.qp
- SVM using the stochastic gradient descent algorithm for optimization<br/>

For implementing the Hard SVM learning rule, the dataset needs to be made linearly separable by removing some of the training points. For each experiment, identify the training data points which are the support vectors.  <br/>
For the soft SVM formulation conduct experiments with different values of the regularization parameter and interpret the results in terms of number of support vectors, margin value, training data and test data classification accuracy.<br/>


**4. Adaboost**<br/>
Implement the Adaboost classifier for classifying examples in a 2D space. You can randomly generate examples in a limited region of the 2D space. Arbitrarily assign binary labels {-1, +1} to the examples. Train Adaboost using the weak hypothesis class as decision stumps in either of the feature axes of the 2D space. Vary the number of stages of Adaboost and note the effect on the performance. Also plot the decision boundary formed by the output hypothesis of Adaboost. Facilitate visualization of the training examples, their labels and the decision boundary. Prepare a report describing the experiments conducted, observations and interpretations. Your implementation should include the explicit steps of learning the weak classifier at each stage, computing the error rate of the weak classifier, updating the weight distribution for the examples after every stage and finally formulating the halfspace over the predictions of the weak classifiers.


**5. K means, GMM and PCA**<br/>
Using a suitable dataset, apply the K-means algorithm for various values of k and choose an appropriate number of clusters using the Silhoutte Score.<br/>
Obtain Gaussian clusters on the same dataset by using GMM. For EM algorithm, initialize the centroid positions using K-means.<br/>
Use PCA to project the data on two dimensions and visualize the clustering output for both Kmeans and GMM.<br/>
For GMM, compare the results for various forms of the Covariance matrix (Full, diagonal, identity).<br/>


**6. Neural Network using PyTorch**<br/>
Implement a Neural Network using PyTorch for the following:
- Classification task 
- Regression task.

Use a dataset of your choice and report the results with different architectures (i.e. changing the number of nodes, layers etc).<br/>
Plot the accuracy on the validation set and the training set as a function of the training epoch number. 

