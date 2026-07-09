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
                sh 'mvn clean compile'
            }
        }

         stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
        
         stage('package') {
            steps {
                sh 'mvn package'
            }
        }
        
    }
}
