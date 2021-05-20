pipeline {
  agent any
  stages {
    stage('Cloning Git') {
      steps {
          git credentialsId: 'github', url: 'https://github.com/Alok018/Jenkins'
         }
      }
    
  stage ('Email Notification'){
    mail bcc: '', body: 'Thanks', cc: '', from: '', replyTo: '', subject: 'Jenkinsjob Successful', to: 'alok.natheee@gmail.com'
     }
  }
}
  
  

