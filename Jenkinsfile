 pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
              sh 'aws --version'
            }
        }
     
             stage('List pods') {
    withKubeConfig([credentialsId: 'KUBECONFIG',
                    caCertificate: '<ca-certificate>',
                    serverUrl: 'https://27451E4791D9E192B83ACF0338944894.gr7.us-west-2.eks.amazonaws.com',
                    contextName: '<context-name>',
                    clusterName: 'eks-1',
                    namespace: '<namespace>'
                    ]) {
              sh 'kubectl get pods'
            }
        }
    }
 }
