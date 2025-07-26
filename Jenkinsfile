pipeline {
    agent any
    tools {
        maven 'Maven3'
    }
    stages {
        stage ('Validate') {
            steps {
                sh 'mvn validate'
            }
        }
        stage ('Compile') {
            steps {
                sh 'mvn compile'
            }
        }
        stage ('Test') {
            steps {
                sh 'mvn test'
            }
        }
        stage ('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}

