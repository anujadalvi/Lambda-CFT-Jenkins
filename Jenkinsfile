pipeline{
	agent any
	stages{
	stage('Clone Repo') {
		steps {
			sh "export AWS_DEFAULT_REGION=us-east-1"
			sh "aws cloudformation create-stack --stack-name ${stackname} --template-body file://lambda_cft.json --parameters ParameterKey='functionname',ParameterValue='${params.Funcname}' --region 'us-east-1'"
			}
	}
		
	
	}
}
