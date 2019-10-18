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
                bat 'npm install'
            }
        }

	stage('Code Review') {
          steps {
               bat  'npm run sonar' 
           }
        }
       
    }
}
   
