pipeline {
    agent any

    stages {
        stage("Build"){
            steps {
                echo 'Build ...'
            }
        }
        stage("Deployment production"){
            when {
                branch "prod"
            }
            steps {
                echo 'Deploy ...'
            }
        }
    }
}