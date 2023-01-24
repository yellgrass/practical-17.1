# practical-17.1

Link to notebook:
https://github.com/yellgrass/practical-17.1/blob/main/prompt_III.ipynb

Findings Summary:

After exploring the data, I initially processed only the first 7 columns pertaining to client data as per the assignment's instructions. I dropped unknown values in all columns as there were not too many and they would also be less useful than an actual value. After dropping these rows, I used onehotencoder and ordinalencoder to represent the categorical variables numerically. From this, I ran basic model of each of the four Logistic Regression, KNN, Decision Tree and SVC, as well as prepared a baseline model of simply always guessing that the client will not subscribe. Although I found very little difference between the models at that point, I decided to use F1 as an evaluation metric after realizing that the data was extremely skewed towards clients deciding not to subscribe, and used that and time to determine what I found to be the best performing model.

Overall, I found the Logistic Regression Model to be the best performing model in terms of predicitve ability combined with time efficiency, as it was very close to the best model (SVC) in terms of F1 score, but far quicker. 
