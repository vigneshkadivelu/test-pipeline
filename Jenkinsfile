pipeline {
  agent {
    kubernetes {
     yamlFile 'build-pod.yaml'
    }
  }
  stages {
    stage('Build') {
      steps { 
         container('maven') {
           script {
          // no container directive is needed as the maven container is the default
        sh "mvn clean package"   
      }
    }
  }
  } 
 }
 }
