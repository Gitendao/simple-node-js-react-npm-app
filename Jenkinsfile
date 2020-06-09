pipeline {
    agent {
        node {
            label 'node'
            customWorkspace 'd/Jenkins/workspace'

        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'npm install' 
            }
        }
    }
}