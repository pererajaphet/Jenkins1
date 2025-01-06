pipeline {
    agent {
        docker {
            image "node:21alpine"
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