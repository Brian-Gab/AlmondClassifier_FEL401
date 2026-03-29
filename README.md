# AlmondClassifier_FEL401
Final project for FEL401 - Machine Learning.


# ========================================================
# MACHINE LEARNING GROUP ACTIVITY
## End-to-End Machine Learning Using a Real-World Dirty Dataset from Kaggle

### Activity Overview
In this activity, you will work as a group to perform a complete machine learning workflow using a real-world dataset from Kaggle. The dataset must be dirty or imperfect, meaning it contains missing values, duplicate rows, inconsistent values, or messy data. You will clean the dataset using Pandas, prepare it for machine learning, train a model, evaluate its performance, and visualize the results. 

### Group Requirements 
- Maximum of 5 members per group 
- All members must participate in the project and presentation 
- Each member must speak during the presentation 

### Main Task 
Find a dirty dataset from Kaggle and build a machine learning project using a Jupyter Notebook. You must perform data cleaning, data preparation, model training, evaluation, and visualization. 

### Required Outputs 
1. Jupyter Notebook containing the full project 
2. Dataset file used 
3. Screen-recorded presentation 
4. Group presentation (all members must speak) 

### Step-by-Step Instructions 
1. Find a dirty dataset from Kaggle. 
2. Inspect the dataset using Pandas (head, info, describe). 
3. Identify data problems (missing values, duplicates, etc.). 
4. Clean the data using Pandas (fillna, dropna, drop_duplicates, etc.). 
5. Prepare the data (features and target selection). 
6. Split the data into training and testing sets. 
7. Train at least one machine learning model. 
8. Evaluate the model using appropriate metrics. 
9. Create visualizations to explain the data and results. 
10. Interpret and explain your results. 

### Suggested Models 
#### Classification: 
- Logistic Regression 
- Decision Tree 
- KNN 
- Random Forest 
 
#### Regression: 
- Linear Regression 
- Decision Tree Regressor 
- Random Forest Regressor 

### Evaluation Metrics 
#### Classification: 
- Accuracy 
- Confusion Matrix 
 
#### Regression: 
- MAE 
- MSE 
- R² Score 

### Presentation Requirements 
- Explain dataset and problem 
- Show data cleaning process 
- Explain model and results 
- Show visualizations 
- All members must present 

### Rubric (100 Points) 
- Dataset Selection – 15 pts 
- Data Inspection – 15 pts 
- Data Cleaning – 20 pts 
- Data Preparation – 15 pts 
- Model Training & Metrics – 15 pts 
- Visualization – 10 pts 
- Notebook Quality – 5 pts 
- Presentation – 5 pts

# ========================================================
# Information about this project

## General Details
This is a simple almond classifying program that uses the sklearn library of python. It uses the real-world almond dataset from Sohaib Moradi on Kaggle.com.

## About the Dataset
Almonds exhibit remarkable diversity. Each almond variety has distinct characteristics, which makes identifying and utilizing them a practical endeavor.
The features are extracted using Image processing techniques following these steps:

1. Converting to HSV color space instead of RGB
2. Creating a mask for brown color
3. Finding edges using Canny
4. Finding contours
5. Drawing contours on the mask
6. Applying the mask to the original image

| Feature Name  | Description                          |
| :------------ | :----------------------------------- |
| Length (major axis)   |   Length of the almond in the image (based on number of pixels) |
| Width (minor axis)    |   Width of the almond in the image (based on number of pixels) |
| Thickness (depth) |   Thickness of the almond in the image (based on number of pixels) |
| Area	|   The area of the Almond region detected in the image |
| Perimeter	|   Total length of the almond boundary |
| Roundness	|   Roundness of the almond: 4 * area / ( π * length ** 2) |
| Solidity	|   Area / area_hull |
| Compactness	|   perimeter**2 / (4 * π * area) |
| Aspect Ratio	|   Length / Width |
| Eccentricity	|   sqrt(1 - ( Width / Length ) **2 ) |
| Extent	|   Area / area_bbox(bounding box) |
| Convex hull(convex area, or area hull)    |	smallest convex set that contains bounding points |
| Type	|   Almond Type |

## Technicals
The training model used for this program is the Logistic Regression under Classification since it is more suitable for non-numerical prediction. 
The dataset is divided into 80% Training and 20% Testing Data.

to be continued...