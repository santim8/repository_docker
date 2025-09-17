pipeline {
    agent any
    stages {
        stage("verify tooling") {
            steps {
                docker --version
                docker version
                docker-compose --version
                echo 'echo Test' 
            }
        }
    }
}
