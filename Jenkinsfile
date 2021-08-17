pipeline {
    agent any

    stages {
        stage('Prepare') {
            steps {
                echo 'Prepared env'
            }
        }

        stage('Build') {
            steps {
                echo "Account name: ${params.name}"
                echo "Account email: ${params.email}"
                echo "Role: ${params.role}"
            }
        }
    }

}