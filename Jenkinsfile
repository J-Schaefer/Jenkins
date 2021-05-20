node{
  stage ('SCM Checkout'){
    git 'https://github.com/Alok018/Jenkins'
  }
  stage ('Email Notification'){
    mail bcc: '', body: 'Thanks', cc: '', from: '', replyTo: '', subject: 'Jenkinsjob Successful', to: 'alok.natheee@gmail.com'
  }

}
