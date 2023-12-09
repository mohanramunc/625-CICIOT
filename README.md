# 625-CICIOT
IOT traffic analysis and attack detection using on-device ML model with Local Deployment

An INLS 625 PROJECT!

A robust model that can accurately distinguish between various types of network activities, including benign and malicious traffic.

Data Preprocessing

Combining and Downsampling: The 49 M, 169 parts csv dataset was downsampled to a target size of 1,000,000 records to balance class distribution.

Data Splitting: The downsampled dataset was split into training and testing sets.

Scaling: The MaxAbsScaler was used for feature scaling to normalize the dataset.

Feature Analysis
The dataset contains 47 features, including flow_duration, Header_Length, Protocol Type, etc.
Basic statistical analysis revealed insights into feature distributions and variations.

Model Training: Logistic Regression model with max_iter=8000.
34 Classes: Original class labels from the dataset.
8 Classes: Labels were consolidated into broader categories like DDoS, DoS, Mirai, Recon, Spoofing, Benign, Web, and BruteForce.
2 Classes: Binary classification into 'Attack' and 'Benign'.

Performance of the models was evaluated using:

Accuracy Score
Recall Score
Precision Score
F1 Score

Exploratory Data Analysis (EDA)
Correlation Matrix: Assessed feature interdependencies.
PCA Analysis: Performed for multivariate analysis.
Anomaly Detection: Identified outliers using Isolation Forest.
Label Encoding: Analyzed label correlations.
Distribution and Box Plots: Visualized feature distributions and outliers.
