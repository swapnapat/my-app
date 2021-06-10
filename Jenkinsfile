node{
	stage('SCM Checkout'){
		
	    git branch: 'main', credentialsId: 'githubcredential', url: 'https://github.com/swapnapat/my-app.git'
    }
	stage('Compile-Package'){
		def mvnHome = tool name: 'maven3', type: 'maven'
		sh  "${mvnHome}/bin/mvn package"
	 }
 }
 
