pipeline {
    agent any
    stages {
        stage('Checkout from GitHub') {
            steps {
                script {
                    // Checkout the code from GitHub
                    checkout scm
                }
            }
        }
        stage('Build') {
            steps {
                // Clean and package the project using Maven
                sh 'mvn clean package'
            }
        }
    }
}
