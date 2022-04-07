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
        git([url: 'https://github.com/Aishwarya-S-Prakash/docker-demo.git', branch: 'master'])
      }
    }
    
  stage('Building image') {
      steps{
        script {
          dockerImage = docker.build imagename
        }
      }
    }
}
