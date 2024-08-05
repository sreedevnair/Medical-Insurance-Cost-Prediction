# Predicting Medical Insurance Cost

In this Project, we will try to predict the insurance cost of person based on the person's details like age, BMI, is that person a smoker, etc.

We will be using Linear Regression model to train and predict the insurance cost.

## Notes :-

### 1. `sns.distplot()`
It stands for Distribution Plot and is used for plotting distributions of continuous variables, mainly through a *histogram*.

### 2. `sns.countplot()`
It is used for visualizing the count of observations in each category of a categorical variable, mainly through bar *graph*.

### 3. `.value_counts()`
It used to the see the counts of every possible values of a feature.

### 4. Data Pre-processing
For data pre-processing, we use `.replace()` function. Inside, first we need to pass a dictionary. Inside this dictionary, we use *column* name as *keys* and another set of dictionary as it's *value*. Inside the nested dictionary, we pass the original values of that column as *keys* and the new data that we want to replace it as the *value*.

### 5. Data Splitting
First, we create the *feature DataFrame* by dropping the target column, which is **charges** from the original DataFrame and saving it in a new DF. Then we create a *target Series* by only selecting the target column and saving it in a new DF.

Then we use the Seaborn's function `.train_test_split()` to split the dataset into traing dataset and testing dataset.

### 6. Training and Evaluating Model
Once we have splitted our data, we will train our model using LinearRegression() class.

We train and predict the model in the same way we train Decision Tree model or Random Forest model.

For evaluating the model, we have used the error metrics known as R squared error. The value of R-square lies between 0 to 1.

When we get R-square equals 1 when the model perfectly fits the data and there is no difference between the predicted value and actual value.

However, when we get R-square equals 0 when the model does not predict any variability in the model and it does not learn any relationship between the dependent and independent variables.

<br>

--------
