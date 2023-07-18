pipeline {
    agent {
        any
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
}
