pipeline {
    agent any 
    stages {
        stage('----clean----') { 
            steps {
			    
				bat "mvn clean -f firstjenkinsmvngithub"
            }
        }
        stage('----Test----') { 
            steps {
                bat "mvn test -f firstjenkinsmvngithub"
            }
        }
        stage('----Deploy----') { 
            steps {
                bat "mvn package -f firstjenkinsmvngithub" 
            }
        }
    }
}