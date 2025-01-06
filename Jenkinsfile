pipeline {
    agent any

    environment {
        DEPLOY_TO = 'production'
    }
    stages {
        stage("Build"){
            steps {
                echo 'Build ...'
            }
        }
        stage("Deployment production"){
            when {
                branch "master"
                environment name: 'DEPLOY_TO' value: 'production'
            }
            steps {
                echo 'Deploy ...'
            }
        }
    }
}