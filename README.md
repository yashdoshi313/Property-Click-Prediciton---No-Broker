# Property-Click-Prediciton---No-Broker

This project focuses on studying and modeling the interactions received by properties listed on NoBroker. The goal is to develop a predictive model that can estimate the number of interactions a property will receive within a specified time frame after its activation. There are some points in the data that need cleaning and transformation in order to predict the clicks on each property. 

## Project Overview

Properties form a critical data entity in the NoBroker ecosystem, where each property can receive multiple interactions, defined as a user requesting an owner's contact. This project aims to build a predictive model to forecast the number of interactions a property will receive within 3 days and 7 days of its activation. However, the time intervals can be customized based on the analysis approach. In this case look into the ipynb file attached to understand what is done in the project.

## Key Objectives

1. **Predictive Modeling**: Develop a model to predict the number of interactions (clicks) a property will receive within a given timeframe after activation.
2. **Data Cleaning and Preparation**: Handle and clean the datasets, including fixing corrupted JSON strings in the property photos data.
3. **Feature Engineering**: Engineer relevant features from the provided datasets to improve the predictive power of the model.
4. **Exploratory Data Analysis (EDA)**: Conduct a thorough EDA to understand the data distributions, relationships, and potential outliers.

## Data Description 

The project uses three primary datasets:

1. **property_data_set.csv**:
   - Contains property features such as activation_date, BHK type, locality, property size, property age, rent, and apartment type.
   - Binary fields like lift and gym indicate the presence (1) or absence (0) of these amenities.

2. **property_photos.tsv**:
   - Contains photo counts of properties.
   - The `photo_urls` column contains corrupted JSON strings that need to be cleaned to determine the number of photos uploaded for each property.
   - Null values indicate the absence of photos for a property.

3. **property_interactions.csv**:
   - Contains timestamps of interactions on properties.
   - The `request_date` field represents the timestamp when a user requested the owner’s contact information, indicating an interaction.

## Methodology Used

1. **Data Cleaning**:
   - Correct the corrupted JSON strings in the `property_photos.tsv` file to count the number of photos uploaded for each property.
   - Merge the datasets to create a comprehensive dataset for modeling.

2. **Exploratory Data Analysis (EDA)**:
   - Visualize and analyze the distribution of interactions, property features, and other relevant data points.

3. **Feature Engineering**:
   - Generate new features from the existing data to enhance the predictive model's accuracy.

4. **Model Building**:
   - Experiment with various predictive models to forecast the number of interactions a property will receive.
   - Evaluate model performance based on standard metrics.

5. **Results and Conclusion**:
   - Present the results of the predictive modeling.
   - Discuss the findings and potential improvements.

## Tools and Technologies Used

- **Python**: For data manipulation, analysis, and modeling.
- **Pandas**: For data cleaning and preparation.
- **NumPy**: For numerical operations.
- **Matplotlib/Seaborn**: For data visualization.
- **Scikit-learn**: For building predictive models.
