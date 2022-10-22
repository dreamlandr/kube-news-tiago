pipeline {
    agent any

    stages{

        stage ('Build Docker Image')
            steps{
                script{
                    dockerapp = docker.build("dreamlander/kube-news-tiago:v1", '-f ./src/dockerfile ./src')
                }
            }

    }


}