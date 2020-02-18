pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'podman pull registry.access.redhat.com/rhscl/python-36-rhel7'
                sh 'python --version'
                
            }
        }
    }
}
