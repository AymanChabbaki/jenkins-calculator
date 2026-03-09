pipeline {
    agent any
    
    tools {
        nodejs 'NodeJS' 
    }

    stages {
        stage('Install Dependencies') {
            steps {
                bat 'npm install' 
            }
        }
        stage('Test') {
            steps {
                bat 'npm test'
            }
        }
        stage('Build') {
            steps {
                echo 'Building the application...'
            }
        }
    }
    post {
        success {
            echo "Bravo, déploiement réussi !"
        }
    }
}