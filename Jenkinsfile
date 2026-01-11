pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build Docker Images') {
            steps {
                sh 'docker compose build'
            }
        }

        stage('CI Status') {
            steps {
                echo 'Docker images built successfully'
            }
        }
    }
}
