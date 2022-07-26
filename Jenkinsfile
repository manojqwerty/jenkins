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
               kubernetesDeploy configs: 'deployment.yaml', enableConfigSubstitution: false, kubeConfig: [path: ''], kubeconfigId: 'kubeconfig555', secretName: '', ssh: [sshCredentialsId: '*', sshServer: ''], textCredentials: [certificateAuthorityData: '', clientCertificateData: '', clientKeyData: '', serverUrl: 'https://']
            }
        }
       }
    }
 }
     
      
