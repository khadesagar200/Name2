pipeline {
    agent any  // Use any available Jenkins agent

    stages {
        stage('Checkout') {
            steps {
                echo 'Cloning the repository...'
                git branch: 'main', url: 'https://github.com/khadesagar200/Name2.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the application...'
                // Simulating a build step
                sh 'echo "Build step executed!"'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                // Simulating a test step
                sh 'echo "Test step executed!"'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                // Simulating a deployment step
                sh 'echo "Deploy step executed!"'
            }
        }
    }

    post {
        always {
            echo 'Pipeline execution complete.'
        }
    }
}
