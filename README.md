# Google-Play-Store-Data-Analysis-and-Prediction-BIG-DATA-
📱 Google Play Store App Rating Prediction
🎯 Project Overview

This project aims to analyze and predict app ratings on the Google Play Store using machine learning techniques in PySpark.
The dataset contains various attributes such as category, price, installs, and content rating, which are used to model the relationship between app characteristics and user ratings.

🧹 Data Preparation

Data Loading & Exploration

Dataset loaded in PySpark, schema inspected to understand structure and data types.

Data Cleaning

Dropped irrelevant columns: Developer Email, Minimum Android, Developer Id, Developer Website, Privacy Policy, Ad Supported, In App Purchases, Editors Choice, Scraped Time, Free.

Casted relevant columns to appropriate types (e.g. float for Rating, Rating Count, Installs, Price).

Filtering Data

Focused on the top 8 app categories:
Education, Music, Business, Tools, Entertainment, Lifestyle, Food & Drink, Books & Reference.

📊 Data Visualization

Category Distribution: Bar & pie charts to show number and percentage of apps per category.

Content Rating Distribution: Count plot to visualize content rating types.

Price Analysis: Identified top 10 most expensive apps and their install counts.

⚙️ Feature Engineering

Encoding Categorical Variables

Used StringIndexer and OneHotEncoder to encode Category and Content Rating.

Vector Assembler

Combined numerical and encoded categorical features into a single vector column (attributes) for model training.

🤖 Modeling & Evaluation

Model-------------------------R²------RMSE------MSE------MAE

Linear Regression------------0.688----1.452----2.108----0.937

Decision Tree Regressor------0.723----1.389------—--------—

Random Forest Regressor-----🏆 0.771---1.278----—--------—

Best Model: Random Forest Regressor

Insights: Feature importance was analyzed to understand which factors most influenced app ratings.

🧠 Results & Conclusion

The Random Forest Regressor outperformed all other models, achieving the highest R² (0.771) and lowest RMSE (1.278).

The model effectively predicts app ratings based on category, installs, and other metadata.

🚀 Future Work

Incorporate user reviews, app descriptions, and sentiment analysis for richer predictions.

Experiment with advanced models like Gradient Boosting, XGBoost, and Neural Networks.

Deploy the model using Flask or Streamlit for interactive use.

🛠️ Tools & Libraries

Language: Python

Framework: PySpark

Libraries: pandas, matplotlib, seaborn, scikit-learn, pyspark.ml

👨‍💻 Author

Muhammad Ali Turk
🎓 Data Scientist | ML & Data Engineering Enthusiast
📫 turk5337@gmail.com
