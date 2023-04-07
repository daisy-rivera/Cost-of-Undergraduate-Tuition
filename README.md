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
   
 #### Average USA Tuition Cost by Year
![Capture](https://user-images.githubusercontent.com/122565297/224843606-a74eef3e-0c32-43ee-b561-9f9a0e70d174.PNG) 
- The data clearly shows that the average cost of tuition is increasing year by year. We can confidently conclude that the cost of tuition will continue to rise in the upcoming years.

### Average Cost by Tuition and Expense Type in USA
![Capture2](https://user-images.githubusercontent.com/122565297/224844265-cc837f94-4593-40bf-8a87-d96bcef0915b.PNG)
- This graph shows the expense by type (Fees/Tuition vs Room/Board) by the type of Tuition (Public In-State, Public Out-of-State or Private). We can see by this graph that Room/Board costs are pretty similar for all types of Tuition. It is the Fees/Tuition expenses that largely differ based on the Type of Tuition.

## Results
-  I utilized various regression metrics to evaluate and compare my models. Overall, the XGBoost and DecisionTree model performed very well. As a final Model I would choose the Decision Tree Model only because it did slightly better than the XGBoost. I had final R2 Test score of .9842 with the DecisionTree Model. 

##Recommendations
- This database does not include information regarding scholarships which can be an additional assett to help future students get a more precise idea of what their costs may be. We can also try to get more specific cost details like cost per credit. It may be helpful as well to gather the index cost of living for each state to see if there is any correlation between the cost of living and the cost of tuition for each state.

### For further information
For any additional questions, please contact **daisy.dinny@hotmail.com**

