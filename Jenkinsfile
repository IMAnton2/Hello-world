pipeline {
    agent any
    stages {
        stage('Build image') {
            steps {
                echo 'Starting to build docker image'
                script {
                    def customImage = docker.build("imanton2/hello-world:0.1")
                    customImage.push()
                }
            }
        }
    }
}
