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
        stage('Yell Foo for me') {
            steps {
                bat 'echo FOO'
            }
        }
        stage('Harry is a nerd') {
            steps {
                bat 'echo BAR'
            }
        }
    }
}
