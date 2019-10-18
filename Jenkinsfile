pipeline {
    agent any
	tools {
        nodejs "node"
    }
	
	
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/vveereshvsh/NodeJsSonar.git'
            }
        }
        stage('Build') {
            steps {
                bat script: 'npm install'
            }
        }

	//	stage('Code Review') {
          //  steps {
               // npm run sonar 
           // }
       // }
       
    }
}
   
