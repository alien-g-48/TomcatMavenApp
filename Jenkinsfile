pipeline {
    agent any
	
	  tools
    {
       maven "Maven"
    }
 stages {
      stage('checkout') {
           steps {
             
                git branch: 'master', url: 'https://github.com/nareshnaresh47/Redbus.git'
             
          }
        }
	 stage('Execute Java Code') {
           steps {
		sh '''
		mvn package
		pwd
		ls -lart
		touch "hello.txt"
		
		
		'''
          }
        }
        

 
     
  
    }
	}
