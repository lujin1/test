pipeline {
  agent any
  stages {
    stage('anchore') {
      steps {
        imageLine = 'lujin525/jenkins-alpinenode:v4'
        writeFile file: 'anchore_images', text: imageLine
        anchore(name: 'anchore_images', bailOnFail: true, engineverify: true, bailOnPluginFail: true, bailOnWarn: true)
      }
    }
  }
}
