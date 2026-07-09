pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/vipinsharma935/mavenproject.git'
            }
        }
       
         stage('Build') {
            steps {
                bat 'mvn clean compile'
            }
        }
        
         stage('Test') {
            steps {
                bat 'mvn test'
            }
        }
        
         stage('package') {
            steps {
                bat 'mvn package'
            }
        }
        
        
        
    }
}
