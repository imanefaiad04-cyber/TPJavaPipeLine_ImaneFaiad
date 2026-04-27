pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                echo ' GitHub'
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Compilation'
                bat 'mvn clean package -DskipTests'
            }
        }

        stage('Test') {
            steps {
                echo 'Tests'
                bat 'mvn clean package -DskipTests'
                bat 'mvn test'
            }
        }
    }

    post {
        success {
            echo ''
        }
        failure {
            echo ' Erreur'
        }
    }
}