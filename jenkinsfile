pipeline {
    agent any

    environment {
        APP_NAME = 'JavaCalculatorApp'
    }

    stages {
        stage('Checkout') {
            steps {
                echo 'Fetching source code from repository...'
                // If using GitHub or Git, uncomment below line:
                // git 'https://github.com/ram-praveen-c/sample.git'
                echo 'Source code checkout complete.'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the project... 🏗️'
                bat 'javac Calculator.java'
                echo 'Build completed successfully.'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests... 🧪'
                bat 'java Calculator'
                echo 'All tests executed successfully.'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the application... 🚀'
                // You can add Docker or file copy commands here if needed
                echo 'Deployment successful! ✅'
            }
        }
    }

    post {
        success {
            echo "🎉 Pipeline completed successfully for ${APP_NAME}!"
        }
        failure {
            echo "❌ Pipeline failed. Check logs for errors."
        }
    }
}
