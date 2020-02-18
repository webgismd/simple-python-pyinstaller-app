pipeline {
    agent { 
        kubernetes {label python}
    }
    stages { 
        stage('build') {
              steps {
                 sh 'python --version'
              }            
        }
    }
}
