
Overview

In this analysis, we set out to develop and evaluate multiple deep learning neural network models, tailored for the specific needs of Alphabet Soup, a charitable organization. The organization sought an effective predictive model to distinguish successful and unsuccessful applicants among the organizations that receive their funding. To achieve this goal, we harnessed a comprehensive dataset containing an array of attributes associated with charitable organizations and their outcomes following funding.


Results

Data Preprocessing

- Target Variable: The target variable is "IS_SUCCESSFUL," which denotes the success (1) or failure (0) of organizations following funding.

- Features: The models employ various columns, including "APPLICATION_TYPE," "AFFILIATION," "CLASSIFICATION," "USE_CASE," "ORGANIZATION," "STATUS," "INCOME_AMT," "SPECIAL_CONSIDERATIONS," and "ASK_AMT."

- Removed Variables: The "EIN" and "NAME" columns were excluded from the input data, as they are neither targets nor features and do not contribute to the model's predictive power.

Model 1

Architecture:
- One hidden layer with 80 neurons using "relu" activation.
- Output layer with 1 neuron and "sigmoid" activation.

Model Performance:
Loss: 0.5564
Accuracy: 0.7321

Model 2

Architecture:
- One hidden layer with 80 neurons using "relu" activation.
- Additional hidden layers with 40, 20, and 10 neurons, all with "relu" activation.
- Output layer with 1 neuron and "sigmoid" activation.

Model Performance:
Loss: 0.5887
Accuracy: 0.7283

Model 3

- Architecture:
One hidden layer with 128 neurons using "relu" activation.
- Additional hidden layers with 64, 32, and 16 neurons, all with "relu" activation.
- Output layer with 1 neuron and "sigmoid" activation.

Model Performance:
Loss: 0.5726
Accuracy: 0.7282

Summary

- In summary, this analysis entailed creating and assessing three deep learning neural network models for predicting the success of charitable organizations receiving funding. Model 1 achieved an accuracy of 73.21%, while Models 2 and 3 attained accuracies of 72.83% and 72.82%, respectively.

For further improvements:

- Hyperparameter Tuning: Fine-tune hyperparameters like learning rate, epochs, and batch size to explore enhancements in model performance.
- Feature Engineering: Investigate feature engineering techniques for more informative features or better encoding of categorical variables.
- Ensemble Methods: Consider using ensemble methods like random forests or gradient boosting for enhanced predictive power.
- Data Augmentation: If possible, acquire more data or apply data augmentation to increase dataset size and diversity.

The choice of approach should align with Alphabet Soup's specific goals and constraints. Further experimentation and fine-tuning are crucial to meet the organization's requirements for predicting charitable organization success.