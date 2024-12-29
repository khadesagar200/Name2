pipeline {
    agent any  // Run the pipeline on any available agent

    stages {
        stage('Checkout') {  // Clone the repository
            steps {
                git branch: 'main', url: 'https://github.com/khadesagar200/Name2.git'
            }
        }

        stage('Build') {  // Compile the code
            steps {
                echo 'Building the application...'
                // Example for Java projects
                sh 'javac Name.java'
            }
        }

        stage('Test') {  // Run tests
            steps {
                echo 'Running tests...'
                // Example: Simulate test execution
                sh 'echo "Tests Passed!"'
            }
        }

        stage('Deploy') {  // Deploy the application
            steps {
                echo 'Deploying the application...'
                // Example: Simulate deployment
                sh 'echo "Application Deployed!"'
            }
        }
    }

    post {
        always {
            echo 'Pipeline completed.'
        }
        success {
            echo 'Pipeline succeeded.'
        }
        failure {
            echo 'Pipeline failed.'
        }
    }
}
