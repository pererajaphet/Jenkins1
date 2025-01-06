pipeline {
    agent {
        docker {
            image 'node:21-alpine'
        }
    }

    stages {
        stage('Pull Docker Image') {
            steps {
                sh 'docker pull node:21-alpine'
            }
        }
        stage("Build"){
            steps {
                sh 'npm -v'
            }
        }
    }

    post {
        always {
            echo 'always !'
        }
        success {
            echo 'success !'
        }
    }
}