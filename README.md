# Regression
Using Google Colab. to simulate Single Variable Non-Linear regression and Linear Regression


## 1 - Packages ##

Import useful packages for scientific computing and data processing.

**Tasks:**
1. Import numpy and rename it to np.
2. Import pandas and rename it to pd.
3. Import the pyplot function in the libraray of matplotlib and rename it to plt.

References:
- [numpy](www.numpy.org) is the fundamental package for scientific computing with Python.
- [matplotlib](http://matplotlib.org) is a famous library to plot graphs in Python.

**Attention:**
1. After this renaming, you will use the new name to call functions. For example, **numpy** will become **np** in the following sections.


2 - Data Preparation
Prepare the data for regression task.

Tasks: 1. Load data for nonlinear regression. 2. Generate the scatter plot of the data.

Hints: 1. The data file is "data_nonlinear.csv". 2. The data format is as follows: 1st column is X and 2nd column is Y. 3. You may follow the example in class. image.png


3 - Single Variable Nonlinear Regression
Develop a regression model, estimate coefficients with data, and derive the relationship.

Tasks: 1. Establish a relationship between Y and X with a quadratic function. 2. Compute MSE loss with observation-prediction pairs. 3. Implement Gradient Descent (GD) to achieve optimal solution with the learning rate of 0.0001 (1e-4) and 10000 (1e4) epochs. 4. Print out the optimal solution at final step.

Hints:
1. Given the example of linear regression in class, modify the function to an equation for a parabola with coefficients of a , b, and c for qudractic, linear, and constant term. 2. Initialize the model with zero. For example, a=0, b=0, and c=0. 3. It may take 10-15 seconds to finish the running for 10000 steps. Be patient. 4. For debugging, the results of a, b, and c for first five steps are as follows:

Epoch 0: 3.488912736685758   0.4593939415755103   0.06521093094378803 \ Epoch 1: 5.81800545347926   0.7661337489695947   0.1088009417029995 \ Epoch 2: 7.372834350372338   0.9709658360861868   0.13795740783840654 \ Epoch 3: 8.410786101973658   1.1077671078485731   0.15747842285122174 \ Epoch 4: 9.103684946272926   1.19915285072093   0.17056706150341266


4 - Prediction Results
Derive prediction function and generate estmated results.

Tasks: 1. Derive prediction function with the obtained coefficients above. 2. Generate scatter plots for original data pairs X-Y and prediction results X-Y_Pred in the same figure.

Hint: 1. You may follow the example in class materials. 2. An example is shown below.

image.png

5 - Multiple Variables Linear Regression
5.1 Data Preparation
Prepare the data for regression task.

Tasks: 1. Load data for multiple variable linear regression. 2. Generate the 3D scatter plot of the data.

Hints: 1. The data file is "data_two_variables.csv". 2. The data format is as follows: 1st column is X1, 2nd column is X2, and 3rd colum is Y. 3. You may use "mplot3d" in the toolkit of "mpl_toolkits" and import "Axes3D" to faciliate 3D scatter plot. More details can be found in the reference of https://matplotlib.org/mpl_toolkits/mplot3d/tutorial.html

image.png

5.2 Linear Regression
Develop a regression model, estimate coefficients with data, and derive the relationship.

Tasks: 1. Establish a linear function to describe the relationship among Y, X1, and X2. 2. Compute MSE loss with observation-prediction pairs. 3. Implement Gradient Descent (GD) to achieve optimal solution with the learning rate of 0.001 (1e-3) and 10000 (1e4) epochs. 4. Print out the optimal solution at final step.

Hints:
1. Given the example of linear regression in class, modify the function to a linear equation with two independent variables X1 and X2. The coefficients of X1 and X2 are m1 and m2, respectively. The constant term is m3. 2. Initialize the model with zero. For example, m1=0, m2=0, and m3=0. 3. It may take 10-15 seconds to finish the running for 10000 steps. Be patient. 4. For debugging, the results of m1, m2, and m3 for first five steps are as follows:

Epoch 0: 0.6349845934491178   1.2882683998193263   0.13209113882254 \ Epoch 1: 1.1097018259626175   2.2060083749415047   0.23322503472662115 \ Epoch 2: 1.4687357224646898   2.857607583186455  0.31207601324063705 \ Epoch 3: 1.7441469025399132   3.3180978011040723   0.3748801743424812 \ Epoch 4: 1.9589934627466363   3.641409029361893   0.4261209277929197


5.3 - Prediction Results
Derive prediction function and generate estmated results.

Tasks: 1. Derive prediction function with the obtained coefficients above. 2. Generate 3D scatter plots for original data pairs X-Y and prediction results X-Y_Pred in the same figure.

Hint: 1. You may follow the example above. 2. An example is shown below. image.png
