pipeline {
    agent none 
    stages {
        stage('Build') { 
            agent {
                docker {
                    image 'python:3:latest' 
                }
            }
            steps {
                sh 'python -m py_compile hello.py' 
            }
        }
    }
}
