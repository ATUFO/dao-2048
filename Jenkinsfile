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

        stage('error') {
          steps {
            mail(subject: 'twst', body: 'test', to: '2221057667@qq.com')
          }
        }

      }
    }

    stage('docker') {
      withEnv(["DOCKER_HOST = tcp://tttfu.top:2375"]) 
    {
        sh 'docker ps -a'
      
    }

  }
  environment {
    DEPLOY_NAME = 'TEST'
    docker_host = 'tcp://tttfu.top:2375'
  }
}
