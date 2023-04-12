# Average Cost of Undergraduate Tuition in the US by State
## Using Machine Learning to help predict the cost of tuition by state
**Daisy Rivera**: 
### Objective:
This database will help students predict the average cost for Undergraduate school by state and help them make what is probably one of the biggest investments of their life.
### Data:
[Link to original dataset](https://www.kaggle.com/datasets/bhargavchirumamilla/average-cost-of-undergraduate-student-by-state-usa) <br>
- This data is posted on Kaggle and was gathered from the National Center for Education Statistics Annual Digest who publishes an annual Digest of Education Statistics report which includes data regarding education in the U.S. 
- It includes information on the average cost of college in the United States, by state and type of institution from 2013 thru 2021.


### Preprocessing for Machine Learning Models
- Features and Target Values were assigned. In this case Value was our Target.
- The data was split into a training and testing dataset using the default 75/25 split.
- Created a processor to include 2 Pipelines(one for categorical columns and one for numeric columns)
 - For categorical columns:
   - Converted categorical columns into numeric by using the OneHotEncoder
 - For numeric columns:
   - Scaled all numeric columns
 
 ### Machine Learning Models
 - Created 3 Machine Learning models
   - Linear Regression Model
   - Decision Tree Model
   - XGBoost Model
  - Each model was tuned to try and improve the default models
  
  ## Exploratory Data Analysis Visuals
   
 #### Average USA Tuition Cost by Year
![Capture](https://user-images.githubusercontent.com/122565297/230646504-65530aa5-5e67-45fe-84f9-774e9533f6cd.PNG)
- The data clearly shows that the average cost of tuition is increasing year by year. We can confidently conclude that the cost of tuition will continue to rise in the upcoming years.

### Average Cost by Tuition and Expense Type in USA
![Capture2](https://user-images.githubusercontent.com/122565297/230646585-9ac924d0-6bfc-48aa-a9ca-e6ff8ec004ab.PNG)
- This graph shows the expense by type (Fees/Tuition vs Room/Board) by the type of Tuition (Public In-State, Public Out-of-State or Private). We can see by this graph that Room/Board costs are pretty similar for all types of Tuition. It is the Fees/Tuition expenses that largely differ based on the Type of Tuition.

### Other Visuals Explored in Project
- Average Yearly Cost by Expense Type
- Average Cost of Tuition by State
- Average Expense for 2-year VS 4-year Tuition
- 5 Most Expensive States by Expense Type
- 5 Least Expensive States by Expense Type
- Average Cost by Expenses for each USA Region
- Average Cost per Semester by Region


## Results
-  I utilized various regression metrics to evaluate and compare my models. Overall, the XGBoost and DecisionTree model performed very well. As a final Model I would choose the Decision Tree Model with its original columns and default hyperparameters. It performed slightly better than the XGBoost will a final R2 Test score of .9842, MAE of $646 and RMSE of $1071.

## Recommendations
For this project we would definitely need more features to help improve the machine learning model. Some features may include:

- Modality - the format in which courses are delivered
- Scholarships - whether federal or private
- Type of Degree - whether Bachelor's, Masters, Associates, etc.
- Major - Some colleges charge more for specific majors such as Engineering or Nursing
- Cost of Living - we can see if there is any correlation between cost of living in a specific state and tuitions

### For further information
For any additional questions, please contact **daisy.dinny@hotmail.com**

