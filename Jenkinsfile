pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                bat 'javac Helloworld.java'
            }
        }

        stage('Test') {
            steps {
                bat 'java Helloworld'
            }
        }

        stage('Archive') {
            steps {
                archiveArtifacts artifacts: '*.class', fingerprint: true
            }
        }
    }
}
