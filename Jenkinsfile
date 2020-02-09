pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'echo ${params.DEPLOY_NAME}'
      }
    }

  }
  environment {
    DEPLOY_NAME = 'TEST'
  }
}