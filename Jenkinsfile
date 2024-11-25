pipeline {
    agent any
    stages {
        stage('Compile') {
            steps { 
                cd '/var/lib/jenkins/workspace/test' 
                sh 'mvn compile'
            }
        }
        stage('test') {
            steps { 
                sh 'mvn test'
            }
        }
        stage('package') {
            steps { 
                sh 'mvn package'
            }
        }
    }
}
