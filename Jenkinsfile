pipeline {
    agent any

    stages {

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