
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'GitHub code checkout'
            }
        }

        stage('Build') {
            steps {
                echo 'Building application'
                bat 'echo Build successful'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing application'
                bat 'echo All tests passed'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application'
            }
        }
    }
}
