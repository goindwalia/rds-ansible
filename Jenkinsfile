pipeline {
    agent any
    
    parameters {
        
        string(defaultValue: 'us-east-1', description: 'AWS Region Name', name: 'REGION')
        string(defaultValue: 'default', description: 'AWS Subnet Name', name: 'SUBNET')
        string(description: 'AWS VPC Security Group', name: 'VPC_SECURITY_GROUPS')
        
    }

    stages {
        stage('Debug') {
            steps {
                echo "flag: ${params.REGION}"
                echo "flag: ${params.SUBNET}"
                echo "flag: ${params.VPC_SECURITY_GROUPS}"
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
