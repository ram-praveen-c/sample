pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Setting up environment... 🏗️'
                // Use your actual Python path below
                bat '"C:\\Users\\rampraveen\\AppData\\Local\\Programs\\Python\\Python311\\python.exe" --version'
            }
        }

        stage('Test') {
            steps {
                echo 'Running calculator script... 🧮'
                bat '"C:\\Users\\rampraveen\\AppData\\Local\\Programs\\Python\\Python311\\python.exe" Calculator.py'
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
