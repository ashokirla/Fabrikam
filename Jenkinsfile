pipeline {
  agent any
  stages {
    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            build 'freestyle 1'
          }
        }
        stage('QA') {
          steps {
            build 'dummy'
            sleep 10
            powershell 'Start-Sleep -s 100'
          }
        }
      }
    }
  }
}
