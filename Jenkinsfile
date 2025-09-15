pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Build') {
            steps {
                echo "Building..."
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                echo "Running tests..."
                sh 'npm test'
            }
        }
    }
}
