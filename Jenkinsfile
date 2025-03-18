pipeline {
    agent any
    stages {
        stage('Checkout') {          
            steps {
                git branch: "main", url: "https://github.com/AkshatPandey-2004/demo-maven-pipeline.git"
            }
        }
        stage('Build') {
            steps {
                // Use Maven to build your project
                bat 'mvn clean package'
            }
        }
        stage('Test') {
            steps {
                // Run tests if applicable
                bat 'mvn test'
            }
        }
    }
} 
