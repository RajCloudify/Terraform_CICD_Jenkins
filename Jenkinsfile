pipeline {
    agent any

    stages {
        stage('Git') {
            steps {
                git branch: 'main', url: 'https://github.com/RajCloudify/Terraform_CICD_Jenkins.git'
            }
        }
        stage('Terraform init-1') {
            steps {
                sh 'terraform init'
            }
        }
        stage('terraform plan-2') {
            steps {
                sh 'terraform plan'
            }
        }
        stage('terraform apply-3') {
            steps {
                sh 'terraform ${execute} -auto-approve'
            }
        }
    }
}


