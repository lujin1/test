pipeline {
  agent any
  stages {
    stage('anchore') {
      environment {
        imageLine = 'lujin525/jenkins-alpinenode:v4'
      }
      steps {
        anchore(name: 'anchore_images', engineverify: true)
      }
    }
  }
}