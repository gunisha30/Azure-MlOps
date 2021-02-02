# Operationalizing Machine Learning

This project aims to execute an Automated ML pipeline, deploy it and subsequently consume the deployed model. A bank marketing dataset is used and the goal is a classification task. The project is implemented using Azure's ML Studio as well as Python SDK. 

## Architectural Diagram

![image](https://github.com/gunisha30/Azure-MlOps/blob/main/Screenshots/flowchart.png)

## Key Steps

**1. Upload the dataset needed for Classification task.**
![image](https://github.com/gunisha30/Azure-MlOps/blob/main/Screenshots/dataset.png)


**2. Create a new automated ML run providing the required configuration.**

![image](https://github.com/gunisha30/Azure-MlOps/blob/main/Screenshots/automlrundetails.png)

![image](https://github.com/gunisha30/Azure-MlOps/blob/main/Screenshots/automlrundetails2.png)

![image](https://github.com/gunisha30/Azure-MlOps/blob/main/Screenshots/automlrunmodels.png)

![image](https://github.com/gunisha30/Azure-MlOps/blob/main/Screenshots/best-model-accuracy.png)


**3. Choose the best model for deployment. Use Azure Container Instance and enable authentication while deploying. The model will be available in the Endpoints section once it is deployed.**

![image](https://github.com/gunisha30/Azure-MlOps/blob/main/Screenshots/deploy-success.png)


**4. Make necessary changes in the file logs.py to enable Application Insights.** 

![image](https://github.com/gunisha30/Azure-MlOps/blob/main/Screenshots/proof%20of%20app%20insight.png)


**5. Download swagger.json file from Endpoints panel, afterwards run serve.py file to view your model properties on the swagger UI documentation.**

![image](https://github.com/gunisha30/Azure-MlOps/blob/main/Screenshots/docker%20image.png)

![image](https://github.com/gunisha30/Azure-MlOps/blob/main/Screenshots/logspyfile.png)

![image](https://github.com/gunisha30/Azure-MlOps/blob/main/Screenshots/swaggersh.png)

![image](https://github.com/gunisha30/Azure-MlOps/blob/main/Screenshots/service-inputs-swagger.png)

![image](https://github.com/gunisha30/Azure-MlOps/blob/main/Screenshots/swagger-deployedmodel.png)


**6. To consume the model, a file called endpoint.py has to be executed. This file needs some changes to be done namely scoring uri and the key. These details can be found in the Consume section of the Endpoints tab. Finally, run the script to obatin the model's output.**

![image](https://github.com/gunisha30/Azure-MlOps/blob/main/Screenshots/endpointpyfile.png)


**7. The second part of the project is to execute the same aim but this time using Python SDK. Upon running the Jupyter notebook provided [here](https://github.com/gunisha30/Azure-MlOps/blob/main/aml-pipelines-with-automated-machine-learning-step.ipynb), the following can be observed:** 

![image](https://github.com/gunisha30/Azure-MlOps/blob/main/Screenshots/pipeline1.png)

![image](https://github.com/gunisha30/Azure-MlOps/blob/main/Screenshots/pipeline2.png)

![image](https://github.com/gunisha30/Azure-MlOps/blob/main/Screenshots/pipelines%20finished.png)

![image](https://github.com/gunisha30/Azure-MlOps/blob/main/Screenshots/pipeline%20finished%20jupy%20nb.png)

![image](https://github.com/gunisha30/Azure-MlOps/blob/main/Screenshots/jupynb.png)

![image](https://github.com/gunisha30/Azure-MlOps/blob/main/Screenshots/jupynb%20run%20details.png)


## Screen Recording
The steps of this project have been briefly demonstrated in this short screen recording. It can be found [here](https://drive.google.com/file/d/111UbZK_HRux3Z7MkVkE4YsOn6PAH-B5N/view?usp=sharing)
