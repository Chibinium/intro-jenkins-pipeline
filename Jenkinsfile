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
        sh 'java -version'
        sh 'sh \'mvn -v\''
      }
    }
  }
}