pipeline {
    agent { dockerfile true }
    stages {
        stage('Test') {
            steps {
                sh 'echo check'
                sh 'python --version'
                sh 'python myscript.py'
            }
        }
    }
}
