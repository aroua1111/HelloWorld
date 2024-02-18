pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Checkout source code from version control
                git 'https://github.com/aroua1111/helloworld.git'
            }
        }
        stage('Build') {
            steps {
                // Invoke Maven to build the project
                sh 'mvn --version'
                sh 'mvn compile'
            }
        }
        stage('packagin') {
            steps {
                // packaging and create jar file
                sh 'mvn package'

            }
        }
        stage('Test') {
            steps {
                // run test
                sh 'mvn test'

            }
        }
    }
}

