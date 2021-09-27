# Relax Inc. Data Scientist take-home challenge

Relax Inc. makes productivity and project management software that's popular with both individuals and teams. 
Founded by several former Facebook employees, it's considered a great company to work for.

##Project Summary
- Created the target feature of 'is_adopted' from the engagement data by:
    - Grouping by user.
    - Resampling the logins to get the total count per week.
- Adjusted the user data by:
    - Adding the target feature.
    - Filling in missing values.
    - Changing the data types for each column as needed.
    - Removing 2 potentially sensitive fields with names.
    - One hot encoding 3 categorical columns.
- Prepared the data to help avoid overfitting by:
    - Splitting into 80% training and 20% test.
    - Scaling the data.
- Chose to use Random forest for this supervised learning classification problem because:
    - it performs well in a multitude of data situations.
    - it is an efficient way to investigate the importance of a set of features (especially in large data sets).
    - dimensionality reduction helps find relevant details.
- Only evaluated one model because it did extremely well with a F1-score of 96.6%.
- The most import features driving the model's predictions were the last_session_creation_time, creation_time, and invited_by_user_id.