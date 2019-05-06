pipeline {
    agent none 
    stages {
        stage('Build') { 
            agent {
                docker {
                    image 'python:3.6' 
                }
            }
            steps {
                sh 'echo build' 
                sh 'python3 test.py'
            }
        }
    }
}
