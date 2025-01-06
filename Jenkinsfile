pipeline {
    agent any

    environment {
        USERNAME = "Japhet"
    }

    stages {
        stage("Build"){
            steps {
                echo "BRANCH_NAME : ${ env.BRANCH_NAME }"
                echo "CI : ${ env.CI }"
                echo "JENKINS_URL : ${ env.JENKINS_URL }"
                echo "BRANCH_IS_PRIMARY : ${ env.BRANCH_IS_PRIMARY }"
                echo "USERNAME : ${ env.USERNAME }"
            }
        }
    }
}