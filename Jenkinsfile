 pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
              sh 'aws --version'
            }
        }
     stage('Deploying App to Kubernetes') {
      steps {
        script {
         sh 'kubectl cluster-info'
        }
      }
    }
    }
 }
     
      
