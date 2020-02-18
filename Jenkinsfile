pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'wget https://www.python.org/ftp/python/3.6.9/Python-3.6.9.tgz'
                sh 'tar xzf Python-3.6.9.tgz'
                dir("${env.WORKSPACE}/Python-3.6.9"){
                        sh 'pwd'
                        sh 'make altinstall'
                        sh 'configure --enable-optimizations'
                }
                sh 'rm Python-3.6.9.tgz'
                sh 'set'
                sh '$WORKSPACE/Python-3.6.9/python -V'
                sh '$WORKSPACE/Python-3.6.9python -m py_compile $WORKSPACE/sources/add2vals.py sources/calc.py'
            }
        }
        
    }
}
