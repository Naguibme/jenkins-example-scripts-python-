pipeline {
    agent any // Utilise n'importe quel agent disponible

    stages {
        stage('Préparation') { // Étape initiale
            steps {
                echo 'Préparation pour exécuter le fichier batch.'
            }
        }

        stage('Exécution du fichier batch') { // Étape principale
            steps {
                bat 'hello.bat' // Exécute le fichier batch "hello.bat"
            }
        }
    }

    post {
        always {
            echo 'Pipeline terminé.'
        }
    }
}
