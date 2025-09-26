pipeline {
    agent any
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
        stage('test') {
            steps {
                sh 'echo "hello test passed"'
            }
        }
        stage('dockerimage')
        {
            steps {
                sh 'echo "docker image stage"'
               echo "docker image pushed successfully"
                }
            }
        }

        
    }
    