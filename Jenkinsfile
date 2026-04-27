pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                echo 'GitHub'
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Compilation'
                sh 'mvn clean package -DskipTests'
            }
        }

        stage('Test') {
            steps {
                echo 'Tests'
                sh 'mvn test'
            }
        }
    }

    post {
        success { echo 'Success' }
        failure { echo 'Erreur' }
    }
}