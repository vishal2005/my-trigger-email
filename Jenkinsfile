node{
	stage('SCM Checkout'){
	git 'https://github.com/vishal2005/my-trigger-email.git'
	}
	stage('Compile Package'){ 
        def mvnHome = tool name:'maven3.5', type:'maven'
	def antHome = tool name: 'Default', type: 'ant'
	sh  "${mvnHome}/bin/ant --version"
	sh "${mvnHome}/bin/mvn --version"
	sh "${mvnHome}/bin/mvn package"
	}
    
}	


