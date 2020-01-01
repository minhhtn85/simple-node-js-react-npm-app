pipeline {
    agent {
        docker {
            image 'node:8-alpine' 
            args '-p 3000:3000' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'sudo chown -R 122:127 "/.npm"'
                sh 'npm install' 
            }
        }
    }
}