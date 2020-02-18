pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'rm -rf  s2i-python-container'
                sh 'git clone https://github.com/sclorg/s2i-python-container.git'
                sh 'cd s2i-python-container'
                sh  'pwd'
                sh 'cd /var/lib/jenkins/jobs/akqfbv-tools/jobs/simple-python-pyinstaller-app/workspace'
                sh 'ls -l'
                sh 'make build TARGET=rhel7 VERSIONS=3.6'
                sh 'python --version'
                
            }
        }
    }
}
