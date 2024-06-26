pipeline {
    agent any

    tools {
        maven 'Maven'  // Utilise le Maven que vous avez configuré dans les outils globaux de Jenkins
    }

    stages {
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Ajoutez ici les étapes de déploiement
            }
        }
    }
}
