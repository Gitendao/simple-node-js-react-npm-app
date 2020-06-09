pipeline {
    agent {
        node {
            label 'simple-node-js-react-npm-app'
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