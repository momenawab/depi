

pipeline {
    agent any
    environment {
        registry = "docker.io"

    }
    stages {

        stage('Build') {
            steps {
                script {
                    sh 'echo "Building application..."'
                    sh 'ls -la'
                    sh 'echo "Build completed successfully"'
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
    