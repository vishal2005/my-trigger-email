node{
	stage('SCM Checkout'){
	git 'https://github.com/vishal2005/my-trigger-email.git'
	}
	stage('Compile Package'){ 
        def mvnHome = tool name:'maven3.5', type:'maven'
	def antHome = tool name:'Default', type:'ant'
	sh  "${antHome}/ant -version"
	sh "${mvnHome}/bin/mvn --version"
	sh "${mvnHome}/bin/mvn package"
	}
	
	stage('Send Email) {
      mail bcc: '', body: '''Hi Welcome to jenkins email alerts system

           Thanks
           Vishal F''', cc: '', from: '', replyTo: '', subject: 'vishal\'s jenkins job', to: 'vishalf2018@gmail.com'
	      
	      }
    
}	


