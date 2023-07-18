pipeline {
    agent {
        docker {
            image 'node:16-buster-slim'
            args '-p 3000:3000'
        }
    }
    stages {
        stage('Build Stage') {
            steps {
                sh 'npm install'
            }
        }
        stage('Test Stage') { 
            steps {
                sh './jenkins/scripts/test.sh' 
            }
        }
    }
}
