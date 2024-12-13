pipeline {
    agent any // Utilise n'importe quel agent disponible

    stages {
        stage('Préparation') { // Étape pour préparer l'environnement
            steps {
                echo 'Préparation de l’environnement sur Windows'
            }
        }

        stage('Exécution du script Python') { // Étape pour exécuter le script
            steps {
                bat 'python hello.py' // Commande Windows pour exécuter le script Python
            }
        }
    }

    post {
        always {
            echo 'Pipeline terminé sur Windows.'
        }
    }
}
