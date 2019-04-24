pipeline {
  agent any
  stages {
    stage('anchore') {
              imageLine = 'lujin525/jenkins-alpinenode:v4'
        writeFile file: 'anchore_images', text: imageLine
      steps {
        anchore(name: 'anchore_images', bailOnFail: true, engineverify: true, bailOnPluginFail: true, bailOnWarn: true)
      }
    }
  }
}
