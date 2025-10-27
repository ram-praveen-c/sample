pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Setting up environment... 🏗️'
                bat 'python --version'
            }
        }

        stage('Test') {
            steps {
                echo 'Running Calculator... 🧮'
                bat 'python Calculator.py'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application... 🚀'
                echo '✅ Deployment successful!'
            }
        }
    }

    post {
        failure {
            echo '❌ Pipeline failed. Check logs for details.'
        }
    }
}
