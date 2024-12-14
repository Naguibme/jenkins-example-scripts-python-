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
                bat 'python hello.py' // Exécute le fichier python
            }
        }
    }

    post {
        always {
            echo 'Pipeline terminé.'
        }
    }
}
