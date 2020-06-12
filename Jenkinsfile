pipeline {
    agent any
    environment {
        CI = 'true'
    }
    parameters {
        choice(     /*Choice Parameter offers choices to choose from*/
            name: 'LOCKER',
            choices: ['HBCIS','PRIM', 'HTRK', 'DWH'],
            description: 'Lockers to test'
        )
        string(
            name: 'LOCKER_CODE',
            defaultValue: 'e.g HBCIS_01,DWH_02',
            description: A comma-separated list of folders to extract
        )
        booleanParam(       /*checkbox that offers true or false options*/
            name: 'PUSH_CHANGES',
            defaultValue: true,
            description: 'Push changes to target repo on success?'
        )
        text(
            name: 'GOODBYE',    /*multi-line supported text box*/
            defaultValue: 'Didn\'t\nwant\nto\nsay\nanything',
            description: 'A farewell message perhaps?'
        )
        password(       /*Parameter for passing a password value*/
            name: 'PASSWORD',
            defaultValue: 'secret',
            description: 'A secret password'
        )

    }
    stages {
        stage('Build') {
            steps {
                bat 'npm install'
            }
        }
        stage('Summary of Selections') {
            steps {
                echo "Lockers: ${params.LOCKER}"
                echo "Locker codes: ${params.LOCKER_CODE}"
                echo "Push changes to target repo: ${params.PUSH_CHANGES}"
            }
        }
        stage('Goodbye Message') {
            steps {
                echo "${params.GOODBYE}"
            }
        }
    }
}
