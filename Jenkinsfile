pipeline{

      agent any
      tools {
           maven 'maven'
           jdk 'java-11'
       }
        
      stages{

        stage('Clone Repo'){
		 steps{
                      script{
		    	                 git branch: 'main', url: 'https://github.com/Saleemullahpasha/tomcat-application.git'
                      	  }
               	     }  
           
        }
          
        stage('Maven Build'){
		 steps{
                      script{
		    	                sh "mvn clean install"
                      	  }
               	     }  
            
        }
		
       }	       	     	         
}
