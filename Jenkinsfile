pipeline {
    agent any

    tools {
        maven 'Maven3.9.15'
        jdk 'jdk-17'
    }

    stages {
        stage('Build') {
            
            steps {
                bat 'mvn clean package'
            }
        }

        stage('Test') {
            steps {
                bat 'mvn test'
            }
        }
    }
}