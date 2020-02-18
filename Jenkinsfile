pipeline {
   agent { label "jenkins-python" }
    stages {
        stage('build') {
             container('python') steps {
                sh  'pwd'
                sh 'python --version'
                
            }
        }
    }
}
