pipeline {
  agent any 
  stages {         
    stage("Git Checkout"){           
      steps{                
	git credentialsId: 'github', url: 'https://github.com/idilassi/tuto-buildimage.git'                 
	echo 'Git Checkout Completed'            
      }        
    }
}
