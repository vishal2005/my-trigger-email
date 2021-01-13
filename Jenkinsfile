node{
	stage('SCM Checkout'){
	git 'https://github.com/vishal2005/my-trigger-email.git'
	}
	stage('Compile Package'){ 
        def mvnHome = tool name:'maven3.5', type:'maven'
	sh  "ant --version"
	sh "${mvnHome}/bin/mvn --version"
	sh "${mvnHome}/bin/mvn package"
	}
    
}	


