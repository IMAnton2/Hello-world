pipeline {
    agent any
    stages {
        stage('Build image') {
            steps {
                bat '''
                 docker build . -t imanton2/hello-world:0.1
                 docker run -p 80:80 imanton2/hello-world:0.1
                    '''
            }
        }
    }
}
