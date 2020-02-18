pipeline {
   agent { label "jenkins-python" }
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
