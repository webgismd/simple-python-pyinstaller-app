pipeline {
 agent {
      label 'kubernetes' }
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
