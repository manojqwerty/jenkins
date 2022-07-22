 pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
              sh 'aws --version'
            }
        }
     
        stage('deploy to eks') {
            steps {
              sh 'kubectl get pods'
            }
        }
    }
 }
