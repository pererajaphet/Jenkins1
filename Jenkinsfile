pipeline {
    agent {
        docker {
            image "node:21-alpine"
        }
    }

    stages {
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