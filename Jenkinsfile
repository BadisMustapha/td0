pipeline{

      agent any
      tools {
           maven 'maven'
           jdk 'java-11'
       }
        
      stages{

        stage('Clone Repo'){
            git branch: 'main', url: 'https://github.com/Saleemullahpasha/tomcat-application.git'
        }
          
        stage('Maven Build'){
            sh "mvn clean install"
        }
		
       }	       	     	         
}
