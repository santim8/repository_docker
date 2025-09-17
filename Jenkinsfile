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
    }
}
