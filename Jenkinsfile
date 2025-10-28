pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Setting up environment... 🏗️'
                // Use double backslashes for Windows paths
                bat '"C:\\Users\\cramp\\AppData\\Local\\Microsoft\\WindowsApps\\python.exe" --version'
            }
        }

        stage('Test') {
            steps {
                echo 'Running calculator... 🧮'
                bat '"C:\\Users\\cramp\\AppData\\Local\\Microsoft\\WindowsApps\\python.exe" calculator.py'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the application... 🚀'
                echo '✅ Deployment Successful!'
            }
        }
    }

    post {
        failure {
            echo '❌ Pipeline failed. Check logs for details.'
        }
        success {
            echo '🎉 Pipeline completed successfully.'
        }
    }
}
