pipeline {
    agent any
    stages {
        stage('Build et Test') {
            matrix {
                axes {
                    axis {
                        name "PLATEFORM"
                        values 'linux', 'macos', 'windows'
                    }
                    axis {
                        name "BROWSER"
                        values 'firefox', 'chrome', 'safari'
                    }
                }
                stages {
                stage('Build') {
                    steps {
                        echo "construire pour ${ PLATEFORM } - ${ BROWSER }"
                    }
                }
                stage('Test') {
                    steps {
                        echo "construire pour ${ PLATEFORM } - ${ BROWSER }"
                    }
                }
            }
            }
        }
    }
}