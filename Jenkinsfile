 pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
              sh 'aws --version'
            }
        }
     
     stages {
        stage('deploy to eks') {
            steps {
              sh 'kubectl get pods'
            }
        }
    }
 }
