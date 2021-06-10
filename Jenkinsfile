node{
   stage('SCM Checkout'){
      git branch: 'main', credentialsId: 'githubcredential', url: 'https://github.com/swapnapat/my-app.git'
    }
    stage('Compile-Package'){
         def mvnHome = tool name: 'maven3', type: 'maven'
	 sh  "${mvnHome}/bin/mvn package"
    }
	stage ('Email Notification'){
	   mail bcc: '', body: '''Hi Welcome to jenkins email alerts
           Thanks 
           Swapna''', cc: '', from: '', replyTo: '', subject: 'Jenkins Job', to: 'swapnadevops07@gmail.com'
   }
 }
 
