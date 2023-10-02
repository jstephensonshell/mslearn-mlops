# mslearn-mlops
https://microsoftlearning.github.io/mslearn-mlops/documentation/00-script.html

In the experimentation folder, you’ll find a Jupyter notebook that trains a classification model. The data used by the notebook is in the experimentation/data folder and contains a CSV file.

In the src/model folder you’ll find a train.py script which already includes code converted from part of the notebook. It’s up to you to complete it.

Go through the notebook to understand what the code does.
 - Convert the code under the Split data header and include it in the train.py script as a split_data function. Remember to:
 - Remove nonessential code.
 - Include the necessary code as a function.
 - Include any necessary libraries at the top of the script.


### Hint

The split_data function is already included in the main function. You only need to add the function itself with the required inputs and outputs underneath the comment TO DO: add function to split data.
Add logging so that every time you run the script, all parameters and metrics are tracked. Use the autologging feature of MLflow to also ensure the necessary model files are stored with the job run to easily deploy the model in the future.

### Hint

MLflow is an open source library for tracking and managing machine learning models. You can use it to track custom metrics. However, since the current model is trained with the common Scikit-learn library, you can also use autologging. By enabling autologging with mlflow.autolog(), all parameters, metrics, and model files will automatically be stored with your job run. Enable autologging in the main function under TO DO: enable autologging.


### Success criteria
To complete this challenge successfully, you should be able to show:

 - A training script which includes a function to split the data and autologging using MLflow.
