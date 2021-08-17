pipeline {
    agent any

    stages {
        stage('Prepare') {
            steps {
                echo 'Prepared env'
            }
        }

        stage('Build') {
            agent {
                docker {
                    image 'python:3.9'
                }
            }
            steps {
                sh 'python -V'
                echo "Account name: ${params.name}"
                echo "Account email: ${params.email}"
                echo "Role: ${params.role}"
            }
        }
    }

}