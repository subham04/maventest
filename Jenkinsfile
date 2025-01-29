pipeline {
    agent any
    tools {
        maven 'maven' // Use the name given in Global Tool Configuration
    }
    stages {
        stage('Checkout Code') {
            steps {
                git 'https://github.com/your-repo/maven-project.git'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean install'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
    }
}
