pipeline {
 agent {
  kubernetes true
}
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
