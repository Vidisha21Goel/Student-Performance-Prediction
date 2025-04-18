# Student-Performance-Prediction
In the field of education, understanding student performance is crucial for timely intervention and support. Predicting whether a student is likely to pass or fail can help educators, parents, and institutions take appropriate measures to guide students in the right direction.
This project focuses on using machine learning techniques to classify students based on their academic performance and analyze patterns among them. We used the Student Performance Dataset from the UCI Machine Learning Repository, which includes features such as attendance, study habits, previous grades, and other relevant academic indicators.
The primary goal of this project is twofold:
1.	Classification – Predict whether a student will pass or fail using historical academic and behavioral data.
2.	Clustering – Segment students into groups based on similar characteristics, enabling institutions to design more personalized learning or support strategies.
This study not only demonstrates the predictive capabilities of machine learning in education but also emphasizes how data-driven insights can support better academic planning and decision-making.

METHODOLOGY

To build this solution, we followed a structured and practical approach to handle both classification and clustering problems effectively.
We began by importing the dataset and manually uploading it into Google Colab for preprocessing. The dataset initially contained various features related to student academic habits and background. We cleaned the data, encoded categorical variables into numerical format using Label Encoding, and normalized the features using StandardScaler for uniformity.
For the classification part, we defined a new target variable named Pass, derived from the GradeClass column. Students with GradeClass 1 or 2 were considered to have "passed," while those with GradeClass 3 or 4 were considered to have "failed." Using this binary target, we trained a Random Forest Classifier—a robust, ensemble-based algorithm known for its accuracy and resistance to overfitting.
The model was evaluated using metrics such as accuracy, precision, and recall. We also generated a confusion matrix and visualized it using a heatmap to clearly see the distribution of correct and incorrect predictions.
In the second part of the project, we performed clustering to segment the students into meaningful groups. We used the KMeans clustering algorithm, which grouped students based on their academic behavior and performance features. To visualize these clusters effectively, we applied Principal Component Analysis (PCA) to reduce the high-dimensional data into two dimensions. The clusters were then plotted with proper labels and colors to interpret them easily.
This two-step methodology allowed us to both predict outcomes and understand the hidden patterns in student data, giving us both actionable results and analytical insight


OUTPUT / RESULT

The final output consists of both classification and clustering results, presented through printed metrics and visual plots.
For classification, the model achieved measurable scores across various metrics:
•	Accuracy – indicating the overall correctness of the model.
•	Precision – showing how many predicted "pass" cases were actually correct.
•	Recall – reflecting the model’s ability to capture actual pass cases.
The confusion matrix heatmap clearly visualizes the performance of our classifier by comparing actual versus predicted labels. High diagonal values in the heatmap indicate strong model performance.
In the clustering section, students were divided into three distinct clusters. Each cluster groups students with similar traits, such as study habits, past grades, and attendance patterns. The scatter plot

![image](https://github.com/user-attachments/assets/b34ea555-6900-404d-b2f8-e19522273dd3)
![image](https://github.com/user-attachments/assets/5ae1e106-66fc-4d1d-ac35-4731e39c0ee7)
![image](https://github.com/user-attachments/assets/1378476e-0053-4386-bc0b-3988b3e140ba)
