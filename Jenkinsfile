pipeline {
    agent any
    tools {
        maven 'MAVEN3'
    }
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/cloudogu/jenkinsfiles'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn -B package'
            }
        }
    }
}