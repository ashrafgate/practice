pipeline {
    agent {
        node {
            label 'maven'
        }
    }
environment {
    PATH = "/opt/apache-maven-3.9.6/bin:$PATH"
}
    stages {
        stage('CLEAN') {
            steps {
                sh 'mvn clean'
            }
        }
        stage('COMPILE') {
            steps {
                sh 'mvn compile'
            }
        }
        stage('TEST') {
            steps {
                sh 'mvn test'
            }
        }

    }
}