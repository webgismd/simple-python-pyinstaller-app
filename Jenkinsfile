pipeline {
 agent {
    kubernetes {
       label python }
    stages {
        stage('build') {
              steps {
                 container('python'){
                sh  'pwd'
                sh 'python --version'
                 }
            }
        }
    }
}
