node{
	stage('SCM Checkout'){
            
	    git 'https://github.com/rangu35/my-app'
		}
	stage('Compile-Package'){
		def mvnHome = tool name: 'maven-3.6', type: 'maven'
		sh "${mvnHome}/bin/mvn package"		
	}
	stage ('Email'){
	mail bcc: '', body: 'Email notification ', cc: '', from: '', replyTo: '', subject: 'jenkins file email notification', to: 'devops.practice2k19@gmail.com'
	}
	}
