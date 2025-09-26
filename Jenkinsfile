pipeline {
    environment {
        registry = "docker.io"

    }
    stages {

        stage('Build') {
            steps {
                script {
                    docker.build("depi-test")
                }
            }
        }
        
    }