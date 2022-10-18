pipeline {
  agent any 
  stages {         
    stage("Git Checkout"){           
      steps{                
        git branch: 'main', credentialsId: 'credentilas-dockerhub', url: 'https://github.com/idilassi/tuto-buildimage.git'
	      echo 'Git Checkout Completed'            
      }        
    }
	  
    stage('Build Docker Image') {  
      steps{                     
	bat '  docker build -t jenkins-demo:${BUILD_NUMBER} .'     
	echo 'Build Image Completed'                
    }           
} 
}
}
