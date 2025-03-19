pipeline {
    agent any
    stages {
        stage('Checkout') {          
            steps {
                git branch: "master", url: "https://github.com/JayvardhanSinghNegi/SL-MAVEN-8-FEB-BACTH"
            }
        }
        stage('Build') {
            steps {
                // Use Maven to build your project
                sh 'mvn clean package'
            }
        }
        stage('Test') {
            steps {
                // Run tests if applicable
                sh 'mvn test'
            }
        }
    }
} 
