pipeline {
    agent any

    stages {
        stage('confirm version') {
            steps {
                nodejs('node') {
                    sh 'node -v'
                    sh 'npm -v'
                }
            }
        }
        stage('install node packages') {
            steps {
                nodejs('node') {
                    sh 'npm install'
                }
            }
        }
    }
}
