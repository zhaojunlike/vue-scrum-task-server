pipeline {
    agent any
    environment {
       NODE_ENV = 'production'
    }
    stages {
        stage('Build') {
            steps {
                sh "echo 'build success ...'"
                sh 'docker build . -t oeyteam-server:v1'
            }
        }
        stage('Test') {
            steps {
                sh 'echo 2'
            }
        }
        stage('Deploy') {
            steps {
                sh 'npm run deploy'
            }
        }
    }
}
