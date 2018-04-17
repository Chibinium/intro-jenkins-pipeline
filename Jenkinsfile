pipeline {
  agent any
  stages {
    stage('Say hello') {
      steps {
        echo 'Hello ${params.Name}!'
      }
    }
  }
  parameters {
    string(name: 'Name', defaultValue: 'Default User', description: 'Who should I say hi to?')
  }
}