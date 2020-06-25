pipeline {
   	           	         agent any
			tools {
     				   maven 'Maven 3.3.9'
        				  jdk 'jdk8'
	                                         }
                                                stages{
		                       stage('Checkout external proj') {
        		                           steps {
                                                                       git branch: */master',
                                                                       credentialsId: 'creadentials_id',
                                                                       url: 'ssh://git@github.com:aravindchakilam/JaiVinayaka.git'				
                                                                   }
                                                                  }
                                                        stage('compile'){
			          steps {
               		                	     sh 'mvn compile'
            
       			                    }
                                                            }
                                               }
  
