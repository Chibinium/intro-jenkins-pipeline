pipeline {
  agent any
  stages {
    stage('Deploy') {
      input {
        message 'Should we continue?'
      }
      steps {
        echo 'Authorized for ${params.NAME}'
      }
    }
  }
  parameters {
    string(name: 'NAME', defaultValue: 'whoever you are', description: 'Who should I say hi to?')
  }
}