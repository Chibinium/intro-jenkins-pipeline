pipeline {
  agent {
    docker {
      image 'maven:3.5.2-jdk-9'
    }
    
  }
  stages {
    stage('Say hello') {
      steps {
        sh 'echo \'Hello World!\''
      }
    }
    stage('mvn -v') {
      steps {
        sh 'sh \'mvn -v\''
      }
    }
  }
}