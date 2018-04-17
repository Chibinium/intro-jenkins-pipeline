pipeline {
  agent any
  stages {
    stage('Say hello') {
      steps {
        sh 'echo \'Hello ${params.Name}!\''
        sh 'java -version'
        sh '''echo "User: ${TEST_USER_USR}"
echo "Password: ${TEST_USER_PSW}"'''
      }
    }
    stage('Deploy') {
      options {
        timeout(time: 1, unit: 'MINUTES')
      }
      input {
        message 'Should we continue?'
      }
      steps {
        echo 'Continuing with deployment'
      }
    }
  }
  environment {
    MY_NAME = 'Mary'
    TEST_USER = 'credentials(\'test-user\')'
  }
  parameters {
    string(name: 'Name', defaultValue: 'whoever you are', description: 'Who should I say hi to?')
  }
}