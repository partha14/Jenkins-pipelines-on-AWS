# Jenkins-pipelines-on-AWS
Automatically deploy code on S3 using Jenkins pipelines utilizing BlueOcean plugin

<h1>Summary </h1>
The objective is to automatically pick up code (HTML file in this case), run some tests using (Lint) through the use of multi pipelines
on Blue Ocean plugin in Jenkins to then automatically deploy (if the tests are passed) by uploading the file to S3 (in this case). 
This is a demonstration of CI/CD using Jenkins Pipelines on AWS. 

<h1> Code </h1>

<b> Index.html </b>

Contains the html file to be eventually uploaded to the S3 bucket to serve static page for the web application

<b> Jenkinsfile: </b>

Contains the stages and steps to perform some tests using lint and if successful upload to S3 bucket.

