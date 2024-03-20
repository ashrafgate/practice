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
        stage('clean workspace') {
            steps {
                sh 'mvn clean'
            }
        }
    }
}