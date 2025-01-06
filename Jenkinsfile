pipeline {
    agent any

    parameters {
        string(name: 'NAME', defaultValue: 'M. Jenkins', description: 'Qui est-ce ?')
        text(name: 'TEXT', defaultValue: 'Un text', description: 'Une description')
        booleanParam(name: 'TOGGLE', defaultValue: true, description: 'true ou False')
        choice(name: 'CHOISE', choices: ['un', 'deux', 'trois'], description: 'Une liste')
        password(name: 'PASSWORD', defaultValue: "SECRET", description: 'un mot de passe')
    }

    stages {
        stage("Build"){
            steps {
                echo "NAME : ${ NAME }"
                echo "TEXT : ${ TEXT }"
                echo "TOGGLE : ${ TOGGLE }"
                echo "CHOISE : ${ CHOISE }"
                echo "NAME : ${ NAME }"
            }
        }
    }
}