# ML-Workflow

Image classification model that can tell bicycles apart from motorcycles, using AWS sevices.
Final Project of Udacity AWS ML Fundamentals.

1. Data Staging and ETL

- CIFAR dataset 
- Extracted the data from the hosting service
- Transformed it into a usable shape and format
- Loaded it into S3

2. Model training and deployment

- Trained using AWS Image classification algorithm
- Deployed to an endpoint and configured Model Monitor to track the deployment

3. Lambda Functions

- Function 1: Serialize image data
- Function 2: Image classification
- Function 3: Filtering out low-confidence inferences

4. Step Function

- AWS Step Functions to compose the model and services into an event-driven application
- Chained the above three lambda functions

5. Testing and Evaluation

- Captured data from SageMaker Model Monitor used to create a visualization to monitor the model