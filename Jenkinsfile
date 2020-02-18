pipeline {
    agent {
    kubernetes {
      label 'python'
      defaultContainer 'jnlp'
      yaml """
apiVersion: v1
kind: Pod
metadata:
labels:
  component: ci
spec:
  # Use service account that can deploy to all namespaces
  serviceAccountName: jenkins2150
  containers:
  - name: python
    image: registry.redhat.io/rhel8/python-36
    command:
    - python --version
    tty: true
  """
    }}
    stages {
        stage('build') {
            steps {
                sh  'pwd'
                sh 'python --version'
                
            }
        }
    }
}
