pipeline {
  agent any
  stages {
    stage('anchore') {
      environment {
        imageLine = 'lujin525/jenkins-alpinenode:v4'
      }
      steps {
        writeFile file: 'anchore_images', text: imageLine
        anchore(name: 'anchore_images', engineverify: true)
      }
    }
  }
}
