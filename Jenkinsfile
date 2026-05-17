pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                git 'https://github.com/mirdanishalik-creator/7.2CDevSecOps.git'
            }
        }

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

