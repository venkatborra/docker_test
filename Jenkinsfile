pipeline {
    agent any
    stages {
        stage("verify tooling") {
            steps {
                bat '''
                    docker infor
                    docker version
                    docker compose version
                    curl --version
                '''
            }
        }
    }
}
