pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Checking out code from GitHub...'
                checkout scm
            }
        }

        stage('Build Backend') {
            steps {
                echo 'Building backend with Maven...'
                bat 'cd ems-backend && mvn clean package -DskipTests'
            }
        }

        stage('Build Frontend') {
            steps {
                echo 'Building frontend...'
                bat 'cd ems-frontend && npm install && npm run build'
            }
        }

        stage('Docker Build') {
            steps {
                echo 'Building Docker images...'
                bat 'docker build -t employee-backend:v1 ./ems-backend'
                bat 'docker build -t employee-frontend:v1 ./ems-frontend'
            }
        }

    }

    post {
        success {
            echo 'CI pipeline completed successfully!'
        }

        failure {
            echo 'CI pipeline failed. Check the console output.'
        }
    }
}