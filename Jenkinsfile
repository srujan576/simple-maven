pipeline {
    agent any

    stages {
        stage('Validate') {
            steps {
                sh mvn validate
            }
        }
        stage('Compile') {
            steps {
                sh mvn clean compile
            }
        }
        stage('Test') {
            steps {
                sh mvn test
            }
        }
        stage('Build') {
            steps {
                sh mvn clean install
            }
        }
    }
}

