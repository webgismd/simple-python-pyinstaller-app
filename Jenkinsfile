pipeline {
    agent openshift {label 'python'}
    stages {
        stage('build') {
            steps {
                sh  'pwd'
                sh 'python --version'
                
            }
        }
    }
}
