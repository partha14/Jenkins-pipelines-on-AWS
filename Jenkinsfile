pipeline {
    agent any
    stages('Upload to AWS') {
       steps {
        	withAWS(region:'us-west-2', credentials:'aws-static')
            {
            sh 'echo "Uploading content with AWS creds"'
            s3Upload(file:'index.html', bucket:'jenkins-pipeline-on-aws-partha', path:'s3://jenkins-pipeline-on-aws-partha/index.html')

            }
        }
    }
}
