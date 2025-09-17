pipeline {
    agent any
    stages {
        stage("verify tooling") {
            steps {
                bat 'docker --version'
                bat 'docker version'
                bat 'docker-compose --version'
                echo 'echo Test' 
            }
        }
        stage ('Prune Docker data') {
            steps {
                bat 'docker compose up -d --no-color --wait'
                bat 'docker images'
                bat 'docker compose ps'
            }
        }
    }
}
