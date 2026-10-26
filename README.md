# cs82a-portfolio 
My name is Disiree Abel.
I am learning Python, data analysis, and programming through CS82A otherwise known as Computer Science & Information Systems.
This repository contains my coursework and projects from the course. Module 2: Python foundations.
**Findings and Results**

This project explored whether study time and the number of absences could help predict students' final grades. The dataset contained 649 student records. No duplicate rows or missing values were found in the selected columns, so no records were removed during cleaning.

The results showed that students who reported more study time generally had higher average final grades. Students in study-time category 3, representing 5–10 hours of studying per week, had the highest average grade at 13.23 out of 20. Students in category 1, representing less than 2 hours per week, had an average grade of 10.84.

The relationship between absences and final grades was very weak and negative, with a correlation of -0.091. This suggests that absences alone had little linear relationship with final grades in this dataset.

A linear regression model was trained using study time and absences. The model was evaluated on 130 testing records. Its Mean Absolute Error (MAE) was 2.30 grade points, and its R-squared value was 0.04. This means the model explained approximately 4% of the variation in final grades and was not very effective at predicting individual students' grades.

Overall, study time showed a positive association with average final grades, but study time and absences alone were not enough to accurately predict final grades. Other factors, such as previous academic performance, family support, motivation, and learning conditions, may also play a role. These findings show association, not causation.
