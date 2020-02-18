pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'wget https://www.python.org/ftp/python/3.6.9/Python-3.6.9.tgz'
                sh 'tar xzf Python-3.6.9.tgz'
                sh './Python-3.6.9/make altinstall'
                sh './Python-3.6.9/configure --enable-optimizations'
                sh 'rm Python-3.6.9.tgz'
                sh './Python-3.6.9/python -V'
                sh './Python-3.6.9python -m py_compile sources/add2vals.py sources/calc.py'
            }
        }
        
    }
}
