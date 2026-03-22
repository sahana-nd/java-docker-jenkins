pipeline {
    agent any

    stages {

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t java-app .'
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker run java-app'
            }
        }
    }
}