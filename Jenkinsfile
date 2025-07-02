pipeline {
    agent any

    environment {
        APP_NAME = "Weather App"
    }

    stages {
        stage('Checkout') {
            steps {
                echo "Checking out ${APP_NAME} code..."
                // Simulate Git checkout
                sh 'echo git clone https://example.com/weather-app.git'
            }
        }

        stage('Build') {
            steps {
                echo "Building ${APP_NAME}..."
                // Simulate a build step (e.g., npm install, Maven compile, etc.)
                sh 'echo Building files...'
            }
        }

        stage('Test') {
            steps {
                echo "Running tests for ${APP_NAME}..."
                // Simulate test execution
                sh 'echo Running unit tests...'
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploying ${APP_NAME} update..."
                // Simulate deployment (e.g., copy to server, restart service)
                sh 'echo Deploying to production server...'
            }
        }
    }

    post {
        success {
            echo "${APP_NAME} update pipeline completed successfully!"
        }
        failure {
            echo "Something went wrong with ${APP_NAME} update pipeline!"
        }
    }
}
