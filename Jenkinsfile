pipeline {
    agent none
    stages {
        stage('Build') { 
            agent { docker { image 'python:3.7.2' } }

            steps {
                sh 'python -m py_compile sources/add2vals.py sources/calc.py' 
            }
        }
    }
}
