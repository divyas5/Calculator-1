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
                sh 'sudo usermod -a -G docker jenkins'
                sh 'python -m py_compile sources/hello.py' 
            }
        }
    }
}
               
