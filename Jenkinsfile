pipeline {
    agent any
    stages {
        stage("verify tooling") {
            steps {
                sh '''
                    docker infor
                    docker version
                    docker compose version
                    curl --version
                '''
            }
        }
    }
}