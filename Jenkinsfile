pipeline {
    agent any
	tools {
        nodejs "NodeJs12"
    }
	
	
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Build') {
            steps {
                npm install 
            }
        }

	//	stage('Code Review') {
          //  steps {
               // npm run sonar 
           // }
       // }
       
    }
}
   
