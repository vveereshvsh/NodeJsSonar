pipeline {
    agent any
	tools {
        nodejs 'NodeJs12'
    }
	
	
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/vveereshvsh/Jenkins_Sonar.git'
            }
        }
        stage('Build') {
            steps {
                npm install 
            }
        }
		stage('Code Review') {
            steps {
                npm run sonar 
            }
        }
       
    }
}
   
