pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/Balram-Parmar/22bce224_pr8'
            }
        }

        stage('Test Each Service') {
            steps {
               bat 'echo 🧪 Testing Service 1...'
            }
        }

        stage('Deploy') {
            steps {
                bat 'echo 🚀 Deploying using docker-compose...'
               
            }
        }
    }

    post {
        success {
            echo '✅ Build and deployment successful for all services!'
        }
        failure {
            echo '❌ Build failed during testing or deployment.'
        }
    }
}