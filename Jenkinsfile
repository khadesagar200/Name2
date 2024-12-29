pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/khadesagar200/Name2.git'
            }
        }

        stage('Build') {
            steps {
                sh 'javac Name.java'
            }
        }

        stage('Test') {
            steps {
                sh 'java Name'
            }
        }
    }

    post {
        success {
            echo 'Build and Test Successful!'
        }
        failure {
            echo 'Build or Test Failed!'
        }
    }
}
