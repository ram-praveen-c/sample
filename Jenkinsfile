pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Setting up environment... 🏗️'
                bat '"C:\\Users\\cramp\\AppData\\Local\\Microsoft\\WindowsApps\\python.exe" --version'
            }
        }

        stage('Test') {
            steps {
                echo 'Running Calculator.py... 🧮'
                bat '"C:\\Users\\cramp\\AppData\\Local\\Microsoft\\WindowsApps\\python.exe" Calculator.py'
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
        success {
            echo '🎉 Pipeline executed successfully!'
        }
        failure {
            echo '❌ Pipeline failed. Check logs for details.'
        }
    }
}
