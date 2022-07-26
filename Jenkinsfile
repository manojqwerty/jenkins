 pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
              sh 'aws --version'
            }
        }
      stage('K8S Deploy') {
        steps{   
            script {
                withKubeConfig([credentialsId: 'kubeconfig555', serverUrl: '']) {
                sh ('kubectl apply -f deployment.yaml')
                }
            }
        }
       }
    }
 }
     
      
