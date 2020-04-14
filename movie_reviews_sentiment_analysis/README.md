# SageMaker Deployment Project

This project is an application of utilizing SageMaker API and AWS technologies to build a web application that analyzes and classifies the sentiment of movie reviews as "Negative" or "Positive". The web app will have a webpage as a front end that users can interact with and submit their movie reviews to. Once a review is submitted, an API will triger a Lambda function to process the data and pass it along to the model endpoint (which works as an interface to the model). Next, the deployed model on AWS gets invoked to predict the sentiment of the submitted review and returns the result (review sentiment) back to the user through an API to display it on the webpage.

Below is the list of tools/technologies used to complete this project:
 - Amazon SageMaker (ml.m4.xlarge and ml.p2.xlarge instances)
 - Amazon Lambda Functions/service
 - Amazon API Gateway
 - Amazon s3


After creating an instance on AWS SageMaker and deploying the model, below is an example of the sentiment classification result for a positive and negative reviews for the movie Parasite (2019):
![pos]
(./Screen Shot 2020-04-11 at 2.18.02 PM.png)

![neg]
(./Screen Shot 2020-04-11 at 2.19.58 PM.png)