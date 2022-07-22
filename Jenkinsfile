 pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('deploy') {
            steps {
             script {
             kubeconfig(credentialsId: 'kuber', serverUrl: '') {
              sh 'kubectl apply -f deployment.yaml'
             }
             }
            }
        }
    }
 }
