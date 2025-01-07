pipeline {
    agent any
    stages {
        stage('Build et Test') {
            steps {
                echo "Construire et tester l'application."
            }
        }
        stage('Déploiement parallèle') {
            failFast true
            parallel {
                stage('Déploiement Dev') {
                    steps {
                        echo "Déploiement en environnement de développement."
                    }
                }
                stage('Déploiement Staging') {
                    steps {
                        echo "Déploiement en environnement de préproduction."
                    }
                }
            }
        }
    }
}