# Apple qualities
The dataset contains characteristics such as size, weight, sweetness, crispness, juiciness, ripeness, acidity, and quality.
Based on the input numerical data, the model estimates what the quality of the apple will be (good/bad) in the end. 

Data source: [kaggle.com](https://www.kaggle.com/datasets/nelgiriyewithana/apple-quality)

## Dataset
The dataset contains 4000 rows. The parameters are on a -8-to-8-grade scale. Watching them 1-to-1 one cannot see any direct correlation between 2 parameters, that's why I considered I needed to examine it with ML algorithms.

I made a violin plot where one can see the different distributions of the parameters.

## Machine Learning
After the required transformations, I trained the model.
The first method I try is Support Vector Machines, but it did not work well, had an accuracy, precision and recall only around 45-47%.

As a result, I used other methods to make a model. Firstly, I was scaling the features with StandarnScaler.
Then, I made the following methods run:
- Logistic Regression,
- Linear Discriminant Analysis,
- K-Neighbors Classifier,
- Decision Tree Classifier,
- Gaussian Naive Bayes,
- C-Support Vector Classification.

The Decision Tree Classifier turned out to be the best performing model. I ran that model separately as well.
The SVM that I ran first was the slowest and the worst model for each metrics.