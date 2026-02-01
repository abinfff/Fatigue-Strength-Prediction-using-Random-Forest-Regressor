# Fatigue-Strength-Prediction-using-Random-Forest-Regressor
Machine learning model using Random Forest Regressor to predict Fatigue Strength ($10^7$ cycles) based on material properties. Includes feature importance analysis, correlation mapping, and 5-fold cross-validation to identify key mechanical and chemical drivers of material longevity.


🛠️ MethodologyThe analysis follows a standard data science pipeline:Exploratory Data Analysis (EDA): Calculated Pearson correlation coefficients to understand the linear relationships between material features and fatigue strength.Data Preprocessing: * Cleaned metadata (removing indexing columns like Sl. No.).Split the dataset into training (80%) and testing (20%) sets to ensure model generalizability.Modeling: Implemented a Random Forest Regressor, an ensemble learning method that handles non-linear relationships and interactions between features effectively.Validation: * RMSE & $R^2$ Score: Evaluated the accuracy of predictions on unseen data.K-Fold Cross-Validation: Performed a 5-fold "stress test" on the model to ensure stability across different data subsets


.
📊 Key InsightsFeature ImportanceThe project utilizes the Random Forest's internal feature_importances_ attribute to rank variables. Unlike simple correlation, this identifies the actual "drivers" the model used to make accurate predictions.🚀 How to UseClone the repository.Ensure you have pandas, numpy, matplotlib, seaborn, and scikit-learn installed.Run the notebook to visualize the correlation matrix and train the model.
📈 ResultsModel Accuracy 
RMSE for Random Forest: 135.36465854420754
R squared for Random Forest: 0.9854016933798683
Top Predictor:Normalizing temperature,carburaization time



