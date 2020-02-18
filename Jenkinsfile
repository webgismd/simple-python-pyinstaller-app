pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'cd /usr/src'
                sh 'wget https://www.python.org/ftp/python/3.6.9/Python-3.6.9.tgz'
                sh 'tar xzf Python-3.6.9.tgz'
                sh 'cd Python-3.6.9'
                sh 'make altinstall'
                sh './configure --enable-optimizations'
                sh 'rm /usr/src/Python-3.6.9.tgz'
                sh 'pwd'
                sh 'ls -l'
                sh 'python -V'
                sh 'python -m py_compile sources/add2vals.py sources/calc.py'
            }
        }
        
    }
}
