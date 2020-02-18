pipeline {
    agent none
    stages {
        node('python') {
        stage('Build') {
            container('go-agent'){
            steps {
                sh 'pwd'
                sh 'python -v'
                sh 'python -m py_compile sources/add2vals.py sources/calc.py'
            }}
        }}
       
    }
}
