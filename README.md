Overview : This project focuses on building and comparing classification models to predict breast cancer diagnosis (malignant or benign) based on medical imaging features. I cleaned and preprocessed the dataset, scaled features, tuned hyperparameters for the Random Forest model, trained multiple classifiers, and evaluated their performance using accuracy and F1 score metrics. The results were visualized to compare model effectiveness.

Dataset : The dataset contains features extracted from digitized images of breast masses, such as radius, texture, perimeter, area, smoothness, compactness, concavity, symmetry, and fractal dimension. The target variable is the diagnosis, labeled as malignant (M) or benign (B). Non-predictive columns like IDs were removed during preprocessing.

Steps : 
First, I loaded the data and mapped the diagnosis labels to binary values. I removed irrelevant columns and split the data into training and test sets with stratification. Numerical features were standardized using feature scaling to improve model training.

Next, I applied hyperparameter tuning on the Random Forest classifier using GridSearchCV to find the best combination of parameters like number of trees and maximum depth. Logistic Regression and Decision Tree models were also trained for comparison.

Finally, I evaluated the models on the test set using accuracy and F1 score metrics. The results were compared using a bar chart visualization. Additionally, the feature importance from the Random Forest model was plotted to understand which features contributed most to the predictions.
