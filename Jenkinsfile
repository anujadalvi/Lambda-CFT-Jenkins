pipeline{
	agent any
	stages{
	stage('Clone Repo') {
		steps {
			sh "export AWS_DEFAULT_REGION=us-east-1"
			sh "aws cloudformation create-stack --stack-name ${stac_kname} --template-body file://lambda_cft.json --parameters ParameterKey='functionname',ParameterValue='${Function_Name}' --region 'us-east-1'"
			}
	}
		
	
	}
}
