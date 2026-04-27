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
                sh 'mvn clean package -DskipTests'
                sh 'mvn test'
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