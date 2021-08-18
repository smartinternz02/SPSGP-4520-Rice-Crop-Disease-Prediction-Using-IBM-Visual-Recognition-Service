# SPSGP-4520-Rice-Crop-Disease-Prediction-Using-AWS-Cloud-Services
Rice Crop Disease Prediction Using Amazon Rekognition and CloudFormation Service

You can find the training images used for training the model in dataset folder.
The execution screenshots are uploaded in Output images(Proofs) folder.

Project Flow:
1.	Sign up/Sign in to your AWS account.
2.	Create a S3 bucket for storing data(images of rice crop disease).
3.	In Amazon Rekognition Service, create a project with appropriate details. Also, make sure to change the bucket policy as instructed during creation.
4.	Create a dataset with the appropriate name and specifying the s3 bucket path in which images are stored.Make sure to select the checkbox for automatic labelling with respect to the folder in which image is present.
5.	Click on Start Modeling. Choose whether you want to create a new test dataset or split the provided data from s3 bucket into training and test dataset.
6.	After successfull training of the model (training the model will take some time), try deploying the model using either amazon CLI in Amazon Cloudshell or through python.
7.	If you want to test the model yourself using test image, then create a stack in Amazon CloudFormation Service for the api. Make sure to give the following link for Amazon s3 link label. It provides the sample template for checking our Amazon Rekognition models without building UI from scratch.
8.	In the Outputs of the newly created stack, click the url value which will open a new tab where you can start, test and stop the model.
 
Link: https://solution-builders-us-east-1.s3.us-east-1.amazonaws.com/amazon-rekognition-custom-labels-demo/latest/template.yaml

