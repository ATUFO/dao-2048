pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'echo ${DEPLOY_NAME}'
      }
    }

  }
  environment {
    DEPLOY_NAME = 'TEST'
  }
}