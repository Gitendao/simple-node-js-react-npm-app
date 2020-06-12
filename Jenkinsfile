pipeline {
    agent any
    environment {
        CI = 'true'
    }
    stages {
        stage('Build') {
            steps {
                'npm install'
            }
        }
        stage('Yell Foo for me') {
            steps {
                echo 'FOO'
            }
        }
        stage('Harry is a nerd') {
            steps {
                echo'BAR'
            }
        }
    }
}
