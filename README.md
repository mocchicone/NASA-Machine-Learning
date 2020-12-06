# NASA-Machine-Learning
Created supervised machine learning models capable of classifying candidate exoplanets from the raw dataset.  Conducted feature selection and data scaling.  Two classification models, Support Vector and Neural Network, were trained, hyptertuned, and tested.  

## Dataset
Over a period of nine years in deep space, the NASA Kepler space telescope has been out on a planet-hunting mission to discover hidden planets outside of our solar system, otherwise known as  "exo-planets".  The dataset included just under 7000 records classified as either "confirmed", "false positive", or "candidate". 

![nasa](https://github.com/mocchicone/NASA-Machine-Learning/blob/main/Images/exoplanets.jpg)

## Data Preprocessing

Data preprocessing entailed 1) data cleaning, 2) feature selection, and 3) data scaling.  

### Data Cleaning
I dropped any rows with missing values and removed those classified as "candidates" to ensure the model learned on the records that had been correctly classified.  Final dataset had 5,304 records

### Feature Selection
Feature selection allows us to use only the features that have a sizable impact on the classification.  Reducing the features in the model allows for 1) quicker model training, 2) a less complex model, and 3) a reduction in overfitting the model.

I created a correlation matrix heatmap to get a visual of how the features correlated to the outcome variable and eachohter. 
![feature_selection](https://github.com/mocchicone/NASA-Machine-Learning/blob/main/Images/correlation_matrix_heatmap.PNG)

I used the sklearn library to give each feature a score to show it's importance in classification.  Here we can see that KOI_depth variable has the highest score and is the most imporant feature. Based on the scrores I decided to use the top seven features in my model. 
![feature_scores](https://github.com/mocchicone/NASA-Machine-Learning/blob/main/Images/feature_scores.PNG)

## Macine Learning

•	Classification Models: Support Vector and Neural Networks  
•	Hypertune Models  
•	Compare Models  


## Data Source
