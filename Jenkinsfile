pipeline {
  agent any
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