pipeline {
    agent any

    stages {

        stage('Clone Code') {
            steps {
                git 'https://github.com/sahana-nd/java-docker-jenkins.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                script {
                    docker.build("java-app")
                }
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker run java-app'
            }
        }
    }
}