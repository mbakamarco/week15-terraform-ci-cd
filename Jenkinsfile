pipeline {
    agent any

    stages {
        stage('Hinitialize') {
            steps {
                sh 'terraform init'
            }
        }
        stage('format') {
            steps {
                sh 'terraform fmt'
            }
        }
         stage('validate') {
            steps {
                sh 'terraform validate'
            }
        }
        stage('plan') {
            steps {
                sh 'terraform plan'
            }
        }
        stage('apply') {
            steps {
                sh 'terraform apply --auto-approve'
            }
        }
    }
}
