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
           
              bat 'C:\\Users\\nagui\\AppData\\Local\\Programs\\Python\\Python313\\python.exe hello.py'  
            }
        }
    }

    post {
        always {
            echo 'Pipeline terminé.'
        }
    }
}
