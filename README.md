# Operationalizing Machine Learning

This project aims at executing an Automated ML pipeline, deploy it and subsequently consume the deployed model. A bank marketing dataset is used and the goal is a classification task. The project is implemented using Azure's ML Studio as well as Python SDK. 

## Architectural Diagram


## Key Steps
### 1. Create AutoML run and choose best model for deployment:
1. Upload the dataset needed for Classification task.
dataset.png
2. Create a new automated ML run providing the required configuration.
3. Choose the best model for deployment. Use Azure Container Instance and enable authentication while deploying. The model will be available in the Endpoints section once it is deployed.
4. Make necessary changes in the file logs.py to enable Application Insights. 
5. Download swagger.json file from Endpoints panel, afterwards run serve.py file to view your model properties on the swagger UI documentation.
6. To consume the model, a file called endpoint.py has to be executed. This file needs some changes to be done namely scoring uri and the key. These details can be found in the Consume section of the Endpoints tab. Finally, run the script to obatin the model's output.
7. The second part of the project is to execute the same aim but this time using Python SDK.


*TODO*: Write a short discription of the key steps. Remeber to include all the screencasts required to demonstrate key steps. 
*TODO* Remeber to provide screenshots of the `RunDetails` widget as well as a screenshot of the best model trained with it's parameters.

## Screen Recording
*TODO* Provide a link to a screen recording of the project in action. Remember that the screencast should demonstrate:

## Standout Suggestions
*TODO (Optional):* This is where you can provide information about any standout suggestions that you have attempted.
