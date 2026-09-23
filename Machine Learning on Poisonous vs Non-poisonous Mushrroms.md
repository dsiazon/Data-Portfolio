# Machine Learning on Poisonous vs Non-poisonous Mushrroms

## Objectives of the Project

This project explores the use of machine learning classification techniques to distinguish between poisonous and nonpoisonous mushrooms. Using a dataset of 8,124 mushroom samples and 23 physical characteristics, the project evaluates multiple classification models to determine how accurately mushroom toxicity can be predicted.

The analysis focuses on questions such as: How accurately can machine learning predict mushroom toxicity? Which classification techniques perform best? Which mushroom characteristics are most important for prediction? How can model complexity improve performance while minimizing false negatives?

<br />
![](Images/BMS/Mushrooms1.png)

## Analytical Insights

**1. Multiple machine learning models achieved highly accurate classification.**

- Decision Tree, Random Forest, Gradient Boosting, Support Vector Classification, and Logistic Regression were evaluated using different hyperparameters and validation techniques.
- Random Forest, Logistic Regression, and SVC achieved 100% accuracy under their respective final test evaluations.
- Logistic Regression achieved 100% accuracy and recall after tuning, with zero false negatives in the final test set.

**2. Recall was prioritized because false negatives carry a high cost.**

- A false negative occurs when a poisonous mushroom is incorrectly classified as edible.
- Because of the potential consequences of this error, the models were evaluated using recall in addition to accuracy.
- The final Logistic Regression model eliminated the false negatives observed in its initial configuration.

**3. Odor was consistently one of the most important predictors of mushroom toxicity.**

- Odor-related features ranked among the strongest predictors across multiple models.
- The Gradient Boosting model identified odor as its most significant feature, accounting for approximately 61.8% of feature importance.
- Random Forest and Logistic Regression also identified odor-related characteristics as important predictors, demonstrating consistency across different classification approaches.

**4. Model complexity and hyperparameter tuning improved classification performance.**

- The models were tuned by adjusting parameters such as tree depth, number of estimators, regularization strength, kernel, and other model-specific settings.
- For Logistic Regression, increasing the regularization parameter to C = 10 improved performance to 100% accuracy and 100% recall.
- The Random Forest model reached 100% test accuracy at a maximum depth of 7 with 100 estimators.

## Conclusion

The analysis demonstrates that machine learning can effectively classify mushrooms as poisonous or nonpoisonous using their physical characteristics. Multiple classification techniques achieved very high performance, with the final Logistic Regression, Random Forest, and SVC models achieving perfect classification under their respective test evaluations.


Feature analysis also revealed that odor was consistently one of the strongest predictors of mushroom classification across several models. Overall, the project demonstrates how classification algorithms, feature importance analysis, and hyperparameter tuning can be combined to build predictive models while prioritizing the reduction of potentially dangerous false-negative predictions.

![](Images/BMS/Mushrooms1.png)
![](Images/BMS/MushroomsDecisionTree.png)
![](Images/BMS/MushroomsGBC.png)
![](Images/BMS/MushroomsLR.png)
![](Images/BMS/MushroomsRandomForest.png)
![](Images/BMS/MushroomsSVC.png)

