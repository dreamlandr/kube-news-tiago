pipeline {
    agent any
    stages {
        stage ('Build Docker Image'){
            steps {
                script {
                    dockerapp = docker.build("dreamlander/kube-news-tiago:${env.BUILD_ID}", '-f ./src/dockerfile ./src')
                }
            }
        }
    }
}