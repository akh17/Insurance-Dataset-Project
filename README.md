# Insurance-Dataset-Project

Project Summary: The “Insurance Dataset for Predicting Health Insurance Premiums in the US” from Kaggle is a comprehensive collection of data designed to explore factors affecting medical costs and health insurance premiums in the United States.

Primarily, our goals with the dataset are to: Explore and visualize the correlations between various factors that could affect health premiums Find the best model that would be able to predict insurance charges for individuals based on important features from the dataset.

Models and their Peformance:

K-NN a. MSE: 1.6 B. R2: 0.91

Linear Regression a. MSE: 0.13 b. R2: 0.99

SVR a. MSE: 0.15 b. R2: 0.99

Neural Network a. MSE: 0.211

Cluster Linear Regression a. Cluster 0: MSE: 0.089 R2: 0.995 b. Cluster 1: MSE: 0.083 R2: 0.996

Conclusion: Before, our best model as reflected by the scores was linear regression but in comparison, this new model scored better. This also makes sense because clustered linear regression is supposed to improve the accuracy of normal linear regression which is exactly what was reflected in our CLR model.

After further analysis by examining cluster centroids, we found that we could possibly predict what features are contributing to our clusters: Cluster 0: This cluster might represent younger individuals with slightly lower BMI, fewer children, a higher proportion of smokers, more people who never or occasionally exercise, slightly more blue-collar workers and unemployed individuals, and a higher proportion of people with Premium coverage. Cluster 1: This cluster might represent older individuals with slightly higher BMI, more children, a lower proportion of smokers, more people who exercise rarely, slightly more students and white-collar workers, and a higher proportion of people with Standard coverage.

By analyzing these centroids, we can infer that Cluster 0 tends to consist of younger, possibly single individuals or couples without children, with slightly higher smoking rates and are receiving higher insurance coverage. Cluster 1 tends to consist of older individuals, possibly families with children, with slightly lower smoking rates, and are receiving Standard coverage.

These interpretations are useful when trying to predict health premiums and insurance charges.

Relationships between categorical variables and charges: Region does not have a large effect on charges. Regardless of whether the individual is from the southeast, northeast, southwest or the northwest, charges are relatively consistent. Gender does not have a large effect on charges. However, males have a slightly larger insurance charge than females. Smokers have significantly higher charges when compared to non-smokers People with no recorded medical history have the lowest charges, followed by those with high blood pressure, then diabetes. Those with heart disease histories have the highest charges. The same pattern is true for family medical history. Unemployed individuals and students have relatively similar charges, whereas people with white and blue collar occupations have relatively higher charges.
