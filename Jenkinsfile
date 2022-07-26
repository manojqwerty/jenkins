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
              withKubeCredentials(kubectlCredentials: [[caCertificate: '', clusterName: 'eks-1', contextName: 'arn:aws:eks:us-west-2:625258239515:cluster/eks-1', credentialsId: 'KUBECONFIG', namespace: 'default', serverUrl: 'https://27451E4791D9E192B83ACF0338944894.gr7.us-west-2.eks.amazonaws.com']]) {
                   sh 'kubectl get nodes'
              }
              }
            }
        }
      }
    }
     
      
