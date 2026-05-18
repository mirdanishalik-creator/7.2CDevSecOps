pipeline {
    agent any

    stages {

        stage('Install') {
            steps {
                sh 'npm install'
            }
        }

        stage('Security Scan') {
            steps {
                sh 'npm audit || true'
            }
        }

        stage('Build Complete') {
            steps {
                echo 'Pipeline completed successfully'
            }
        }
    }
}
