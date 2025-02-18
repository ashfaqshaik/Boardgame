pipeline {
    agent any
    
    tools{
        maven 'maven3'
        jdk 'jdk17'
    }
    
    
    stages {
        
        
        stage('compile') {
            steps {
                sh "mvn clean compile"
            }
        }
        
        stage('Test') {
            steps {
                sh "mvn clean test"
            }
        }
        
        stage('Build') {
            steps {
                sh "mvn clean package"
            }
        }
    }
}
