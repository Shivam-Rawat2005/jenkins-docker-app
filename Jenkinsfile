pipeline {
    agent any

    stages {
        stage('Build Maven') {
            steps {
                bat 'mvn clean package'
            }
        }

        stage('Build Docker Image') {
            steps {
                bat 'docker build -t maven-app .'
            }
        }
    }
}