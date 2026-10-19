pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
                echo 'GitHub code checkout completed'
            }
        }

        stage('Build') {
            steps {
                echo 'Starting React application build'
                sh 'node --version'
                sh 'npm --version'
                sh 'npm ci'
                sh 'npm run build'
            }
        }
    }
}
