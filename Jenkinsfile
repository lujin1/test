pipeline {
  agent any
  stages {
    stage('anchore') {
      environment {
        imageLine = 'lujin525/jenkins-alpinenode:v4'
      }
      steps {
        sh 'echo "$imageLine" > anchore_images'
        anchore(name: 'anchore_images', engineverify: true)
      }
    }
  }
}