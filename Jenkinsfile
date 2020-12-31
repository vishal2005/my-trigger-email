node{
	stage('SCM Checkout'){
	git 'https://github.com/vishal2005/my-trigger-email.git'
	}
	stage('Compile Package'){ 
        def mvnHome = tool name:'maven3.5', type:'maven'
	sh "${mvnHome}/bin/mvn package"
	}
        stage('Email Notifications'){
        mail bcc: '', body: '''Hi Welcome to Jenkins Email alerts
        Thanks
        Vishal''', cc: '', from: '', replyTo: '', subject: 'Jenkins  Job', to: 'vishalf2018@gmail.com'
		
	}
}	


