pipeline {
    agent any
    tools {
        maven 'MAVEN'
    }

    stages {

        stage('Build Maven') {
            steps{
                 git branch: 'main', credentialsId: 'devopshint', url: 'https://github.com/apraveen005/jenkins-nexus'
                 sh "mvn -Dmaven.test.failure.ignore=true clean package"
                
            }
        }   
 
    }
}
