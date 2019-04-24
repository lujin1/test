pipeline {
  agent any
  stages {
    stage('anchore') {
      steps {
        anchore(name: 'anchore_images', bailOnFail: true, engineverify: true, bailOnPluginFail: true, bailOnWarn: true)
      }
    }
  }
}
