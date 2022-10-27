pipeline {
  agent any
  stages {
    stage('Test') {
      parallel {
        stage('Test 24024') {
          steps {
            build 'freestyle1234'
          }
        }
        stage('QA') {
          steps {
            build 'dummy'
            sleep 10
            releases/M145
            powershell 'Start-Sleep -s 10
          }
        }
      }
    }
  }
}
