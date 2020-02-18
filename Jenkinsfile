pipeline {
     agent { kubernetes {label 'python'} }
    stages {
        stage('build') {
            steps {
                sh  'pwd'
                sh 'python --version'
                
            }
        }
    }
}
