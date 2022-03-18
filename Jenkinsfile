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
  				mvn 'clean install -DskipTests'
                archiveArtifacts '**/target/*.*ar'            }
        }
    }
