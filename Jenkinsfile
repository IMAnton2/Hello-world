pipeline {
    agent any
    stages {
        stage('Build image') {
            steps {
                powershell '''
                 docker build . -t imanton2/hello-world:0.1
                 docker run --detach -p 80:80 imanton2/hello-world:0.1
                    '''
            }
        }
    }
}
