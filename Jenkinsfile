pipeline {
  agent any
  stages {
    stage('Test') {
      parallel {
        stage('Test 24024') {
          steps {
            build 'freestyle123'
          }
        }
        stage('QA') {
          steps {
            build 'dummy'
            sleep 10
            releases/M145
            powershell 'Start-Sleep -s 100
          }
        }
      }
    }
  }
}
