pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the project...'
                sh 'javac Main.java'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                // (Here you can run test commands)
                sh 'echo "All tests passed!"'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                // (You can replace this with real deployment commands)
                sh 'echo "Application deployed successfully!"'
            }
        }
    }

    post {
        success {
            echo '✅ Pipeline completed successfully!'
        }
        failure {
            echo '❌ Pipeline failed. Please check the logs.'
        }
    }
}
