pipeline {
    agent any
    stages {
        stage('Check Docker Image') {
            steps {
                script {
                    def dockerCmd = "/usr/bin/docker"  // Modify the path to the Docker executable
                    sh "${dockerCmd} inspect -f . node:18.18.1-alpine3.18"
                }
            }
        }
    }
}