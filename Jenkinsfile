pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'git clone https://github.com/sclorg/s2i-python-container.git'
                sh 'cd s2i-python-container'
                sh 'make build TARGET=rhel7 VERSIONS=3.6'
                sh 'python --version'
                
            }
        }
    }
}
