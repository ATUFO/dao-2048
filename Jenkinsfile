pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            sh 'echo ${DEPLOY_NAME}'
          }
        }

        stage('') {
          steps {
            mail(subject: 'twst', body: 'test', to: '2221057667@qq.com')
          }
        }

      }
    }

  }
  environment {
    DEPLOY_NAME = 'TEST'
  }
}