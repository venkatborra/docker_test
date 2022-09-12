pipeline {
    agent any
    stages {
        stage("verify tooling") {
            steps {
                bat '''
                    docker version
                    docker info
                    docker compose version
                    curl --version
                '''
            }
        }
        stage('Start mongo db and mongo express containers') {
            step {
                bat 'docker compose -f docker-compose.yaml up -d --no-color --wait'
                bat 'docker compose ps'
            }
        }
    }
}
