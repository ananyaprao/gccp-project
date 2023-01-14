# gccp-project
PROJECT TITLE: Classifying Images of Clouds in the Cloud with AutoML Vision (MIGRATED TO VERTEX AI)
ABSTRACT: Upload images to Cloud Storage and use them for training a custom model to recognize clouds (cumulus, cumulonimbus, etc.).

PROCEDURE:

step 1: set up automl vision
Click on the Cloud AutoML API result and then click Enable.
Create a Cloud Storage bucket for your training data

step 2: Upload training images to Cloud Storage
 Use the gsutil command-line utility for Cloud Storage to copy the training images into your bucket

step 3: Create an AutoML Vision training dataset
Copy the  file to the Cloud Shell instance
Update the CSV with the files in the project
Upload this updated CSV file to the Cloud Storage bucket

step4:Click to open the AutoML Vision datasets page.
At the top of the Cloud Console, click + New dataset.
Type clouds for the dataset name.
Leave Single-Label Classification checked.
Click Create dataset to continue
Select a CSV file on Cloud Storage

step 5: Inspect the images
To see a summary of how many images you have for each label, click on Label stats.

step 6: Train your model
go to the Train tab and click Start training.
Leave Cloud hosted selected and click Continue.
 type the value "8" into the Set your budget * box and check the Deploy model to 1 node after training. 
Click Start training.

step 7: Generate predictions
Navigate to the Test & Use tab in the AutoML UI.
Click Upload images and upload the cloud sample images to test

CONCLUSION:
In this project, I learned how to perform the following tasks:
*To upload a labeled dataset to Cloud Storage and connect it to AutoML Vision with a CSV label file
*Train a model with AutoML Vision and evaluate its accuracy
*Generate predictions on the trained model


