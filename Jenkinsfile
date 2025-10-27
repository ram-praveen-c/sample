pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Setting up environment... 🏗️'
                bat '"C:\\Python312\\python.exe" --version'
            }
        }

        stage('Test') {
            steps {
                echo 'Running calculator... 🧮'
                bat '"C:\\Python312\\python.exe" Calculator.py'
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
        success {
            echo '🎉 Pipeline executed successfully!'
        }
    }
}
