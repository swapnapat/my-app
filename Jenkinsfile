node{
	stage('SCM Checkout'){
	 git 'git branch: 'main', credentialsId: 'githubcredential', 
	      url: 'https://github.com/swapnapat/my-app.git'
    }
	stage('Compile-Package'){
	  sh  'mvn package'
	 }
 }
 
