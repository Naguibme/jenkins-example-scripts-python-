pipeline {
    agent any // Utilise n'importe quel agent disponible

    stages {
        stage('Préparation') { // Étape initiale
            steps {
                echo 'Préparation pour exécuter Le script Python.'
            }
        }

        stage('Exécution du script Python') { // Étape principale
            steps {
           
              bat 'C:\\Users\\nagui\\AppData\\Local\\Programs\\Python\\Python313\\python.exe hello.py' // avec le chemin de Python 
            }
        }
    }

    post {
        always {
            echo 'Pipeline terminé.'
        }
    }
}
