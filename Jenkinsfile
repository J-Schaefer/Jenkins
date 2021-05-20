pipeline {
  environment {
    imagename = "ros_noetic_Dockerfile"
    dockerImage = ''
  }
  agent any
  stages {
    stage('Cloning Git') {
      steps {
          git credentialsId: 'github', url: 'https://github.com/Alok018/Jenkins'
         }
      }
  }
    
    stage('Building image') {
      steps{
        script {
          dockerImage = docker.build imagename
        }
      }
    }
  stage ('Email Notification'){
    mail bcc: '', body: 'Thanks', cc: '', from: '', replyTo: '', subject: 'Jenkinsjob Successful', to: 'alok.natheee@gmail.com'
  }
}
  

