pipeline {
 agent kubernetes {
      label 'openshift' }
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
