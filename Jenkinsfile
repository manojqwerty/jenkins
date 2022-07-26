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
              kubernetesDeploy configs: 'deployment.yaml', dockerCredentials: [[credentialsId: 'docker', url: 'https://hub.docker.com/']], kubeConfig: [path: '/root'], kubeconfigId: 'kubeconfig555', secretName: '', ssh: [sshCredentialsId: 'ssh', sshServer: 'https://27451E4791D9E192B83ACF0338944894.gr7.us-west-2.eks.amazonaws.com'], textCredentials: [certificateAuthorityData: '', clientCertificateData: '', clientKeyData: '', serverUrl: 'https://27451E4791D9E192B83ACF0338944894.gr7.us-west-2.eks.amazonaws.com']
              }
            }
        }
      }
    }
     
      
