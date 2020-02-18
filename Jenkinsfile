pipeline {
    agent none
    stages {
        stage('Build') {
            agent {
                kubernetes {
                    label 'python'
                }
            }
            steps {
                sh 'pwd'
                sh 'python -v'
                sh 'python -m py_compile sources/add2vals.py sources/calc.py'
            }
        }
       
    }
}
