pipeline {
    agent any
    environment {
        CI = 'true'
    }
    stages {
        stage('Build') {
            steps {
                bat 'npm install'
            }
        }
        stage('Foo') {
            steps {
                bat 'echo FOO'
            }
        }
        stage('Bar') {
            steps {
                bat 'echo BAR'
            }
        }
    }
}
