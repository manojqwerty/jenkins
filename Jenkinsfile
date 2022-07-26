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
         sh 'kubectl config use-context arn:aws:eks:us-west-2:625258239515:cluster/eks-1'
        }
      }
    }
    }
 }
     
      
