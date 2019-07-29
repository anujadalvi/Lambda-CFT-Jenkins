pipeline{
	agent any
	stages{
	stage('Clone Repo') {
		steps {
			sh "export AWS_DEFAULT_REGION=us-east-1"
			sh "aws cloudformation create-stack --stack-name dbda4stack --template-body file://lambda_cft.json --region 'us-east-1'"
			}
	}
		
	
	}
}
