pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean install'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
        stage('Deploy') {
            steps {
                // Define deployment steps for your environment (e.g., upload to server)
            }
        }
    }
}
