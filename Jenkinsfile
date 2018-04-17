pipeline {
  agent any
    environment {
    MY_NAME = 'Mary'
    TEST_USER = 'credentials(\'test-user\')'
  }
     parameters {
      string(name: 'Name', defaultValue: 'whoever you are', 
	     description: 'Who should I say hi to?')
   }
  stages {
    stage('Say hello') {
      steps {
        sh 'echo \'Hello ${MY_NAME}!\''
        sh 'java -version'
        sh '''echo "User: ${TEST_USER_USR}"
echo "Password: ${TEST_USER_PSW}"'''
      }
    }
  }

}
