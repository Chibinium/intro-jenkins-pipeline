pipeline {
  agent {
    docker {
      image 'golang:1.10-alpine'
      label 'docker-cloud'
    }
    
  }
  stages {
    stage('Say hello') {
      steps {
        sh 'go version'
      }
    }
  }
}