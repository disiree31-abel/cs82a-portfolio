# cs82a-portfolio 
My name is Disiree Abel.
I am learning Python, data analysis, and programming through CS82A otherwise known as Computer Science & Information Systems.
This repository contains my coursework and projects from the course. Module 2: Python foundations.
Student Performance Analysis

About This Project

For my final project, I wanted to look at whether the amount of time students spend studying and the number of times they miss school can help predict their final grades.

I used Python to look through the data, create charts, and build a simple machine learning model. I wanted to see what patterns I could find and how well the model could predict a student's final grade using just these two factors.

My Research Question

Can a student's study time and number of absences help predict their final grade?

Where the Data Came From

I used the Student Performance Dataset from the UCI Machine Learning Repository.

Dataset: https://archive.ics.uci.edu/dataset/320/student+performance

I used the Portuguese course dataset, called `student-por.csv`. It contains information about students and their school performance.

The dataset is licensed under Creative Commons Attribution 4.0 International (CC BY 4.0).

How I Cleaned the Data

The original dataset had 649 rows and 33 columns. I used pandas to load the data and selected the three columns I needed for my project:

- `studytime`: How much time students spend studying each week, recorded in four categories.
- `absences`: The number of school absences.
- `G3`: The student's final grade, on a scale from 0 to 20.

I also checked for duplicate rows and missing values in the columns I selected. There were no duplicates or missing values to remove, so I kept all 649 records.

What I Found

1. Study Time and Final Grades

Students who reported spending more time studying generally had higher average final grades.

Students in category 1, who studied less than 2 hours per week, had an average grade of 10.84. Category 3, representing 5–10 hours of studying per week, had the highest average grade at 13.23.

Interestingly, category 4, which represents more than 10 hours of studying per week, had a slightly lower average grade than category 3.

Average Final Grade by Study Time

2. Absences and Final Grades

I also looked at whether students who missed more school tended to have lower grades. The correlation was -0.091, which is a very weak negative relationship.

This means that, in this dataset, absences by themselves did not have a strong linear relationship with final grades.

Absences vs. Final Grades

3. Distribution of Final Grades

I created a chart to see how final grades were distributed across the students in the dataset.

The average final grade was 11.91 out of 20, and the most common grade was 11.

Distribution of Final Grades

## Building My Prediction Model

After exploring the data, I used linear regression to see how well study time and absences could predict final grades.

I split the data into two groups. I used 519 records to train the model and 130 records to test it.

The model results were:

- Study time coefficient: 0.966
- Absences coefficient: -0.045
- Mean Absolute Error (MAE): 2.30
- R-squared (R²): 0.04

The MAE means that the model's predictions were off by about 2.3 grade points on average. The R² result means the model explained only about 4% of the variation in grades in the test data.

Actual vs. Predicted Final Grades

Looking at these results, I found that the model was not very good at predicting individual students' grades. Even though study time showed a positive relationship with average grades, these two factors were not enough to make accurate predictions.

My Conclusion

Overall, this project helped me see how data can be used to find patterns and test predictions. I found that students who spent more time studying generally had higher average grades, but the relationship was not exactly the same across every study time category.

I also found that absences had a very weak relationship with final grades in this dataset. When I tested my prediction model, the results showed that study time and absences alone could not explain much of the difference in students' grades.

I think adding more information, such as previous grades, motivation, or other factors that affect learning, could help improve the model. One important thing I learned is that finding a relationship between two things does not necessarily mean one causes the other.

Limitations

There are a few things to keep in mind when looking at my results:

- The data came from Portuguese schools, so the results may not apply to every student or school.
- I only used study time and absences to predict grades.
- Study time was recorded in categories rather than exact hours.
- Other things that may affect grades were not included in my model.
- The model had a low R² value, so it was not very effective at predicting individual grades.

Because of these limitations, I would not use this model by itself to make decisions about a student's academic performance.

Tools I Used

- Python
- pandas
- matplotlib
- scikit-learn
- Jupyter Notebook

How to Run My Project

1. Download the `student-por.csv` dataset from the UCI Machine Learning Repository.
2. Open my notebook in Jupyter Notebook or Google Colab.
3. Make sure pandas, matplotlib, and scikit-learn are installed.
4. Update the file path in the notebook to match where the CSV is saved.
5. Run the notebook cells in order to see the data cleaning, charts, and prediction model results.

**AI Use Disclosure**
I used ChatGPT for help understanding parts of the project and an overall idea of how I can complete the assignment to get the best grade, I also used it for a bit more help with working through Python code, troubleshooting errors ( I received alot and wanted to understand what I was doing incorrect), and organizing my report. I ran the code in my notebook and used the results from my analysis to explain my findings.

