pipeline {
    agent none 
    stages {
        stage('Build') { 
            agent {
                docker {
                    image 'python:2-alpine' 
                }
            }
            steps {
                sh 'echo build' 
                sh 'python3 test.py'
            }
        }
    }
}
