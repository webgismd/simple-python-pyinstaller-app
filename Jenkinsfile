pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'rmdir -f  s2i-python-container'
                sh 'git clone https://github.com/sclorg/s2i-python-container.git'
                sh 'cd s2i-python-container'
                sh 'ls -l'
                sh 'make build TARGET=rhel7 VERSIONS=3.6'
                sh 'python --version'
                
            }
        }
    }
}
