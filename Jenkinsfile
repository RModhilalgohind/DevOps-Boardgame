pipeline {
    agent {lable 'agent-1'}

 tools {
     jdk 'jdk-17'
     maven 'maven3.9'
 }
    
    stages {
        
        stage('Compile') {
            steps {
            sh  'mvn compile'
            }
        }
        
        stage('Testing') {
            steps {
                sh 'mvn test'
            }
        }
        
        stage('Building The Project') {
            steps {
                sh 'mvn package'
            }
        }
    }
}
