pipeline {
  agent any
  stages {
    stage('111') {
      steps {
        echo '22'
      }
    }
    stage('222') {
      steps {
        sh '''ls -l
hostname
ifconfig'''
      }
    }
  }
}