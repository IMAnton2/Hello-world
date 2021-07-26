pipeline {
    agent any
    stages {
        stage('Build image') {
            steps {
                bat '''
                 docker run -p 80:80 hello-world:0.1
                 docker build . -t imanton2/hello-world:0.1
                    '''
            }
        }
    }
}
