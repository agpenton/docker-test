pipeline {
  agent any
  stages {
    stage('Building image') {
      steps {
        sh 'docker.build registry + ":$BUILD_NUMBER"'
      }
    }
  }
  environment {
    registry = '"agpenton/docker-test"'
    registryCredential = 'dockerhub'
  }
}