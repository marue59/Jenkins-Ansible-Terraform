pipeline {
    agent {
        docker { image 'node:10-alpine' }
    }
    stages {
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                sh 'npm test'
            }
        }
        stage('Deploy') {
            steps {
                sh 'docker build -t # .'
                sh 'docker run -it -p 8080:8080 --name # # '
            }
        }
    }
}