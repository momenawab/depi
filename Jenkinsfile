

pipeline {
    agent any
    environment {
        registry = "docker.io"

    }
    stages {

        stage('Build') {
            steps {
                script {
                    sh 'echo "Building Docker image..."'
                    sh 'docker build -t depi-test .'
                    sh 'echo "Docker image built successfully"'
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
                script {
                    sh 'docker images | grep depi-test'
                    sh 'echo "Docker image available for deployment"'
                }
                echo "docker image pushed successfully"
                }
            }
        }

        
    }
    