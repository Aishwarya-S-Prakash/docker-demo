pipeline {
  environment {
    imagename = "aishwaryasp23/jenkins"
    registryCredential = 'dockerhub'
    dockerImage = ''
  }
  agent any
  stages {
    stage('Cloning Git') {
      steps {
        git([url: 'https://github.com/arjunachari12/docker-demo.git', branch: 'master'])
      }
    }
}
