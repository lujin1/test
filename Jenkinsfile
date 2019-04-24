pipeline {
  agent {
    label 'jenkins-maven'
  }
  stages {
    stage('anchore') {
      steps {
        anchore(name: 'anchore_images', bailOnFail: true, engineverify: true, bailOnPluginFail: true, bailOnWarn: true)
      }
    }
  }
}