pipeline {
    agent any
    stages {
        stage('Clone') {
            steps {
                git credentialsId: 'github-token', url: 'https://github.com/Purvi-joshi/jenkins-pipeline-troubleshooting.git'
            }
        }
        stage('Build') {
            steps {
                sh 'echo "Building the Flask App..."'
                sh 'docker build -t flask-jenkins-app .'
            }
        }
        stage('Test') {
            steps {
                sh 'echo "Run tests here (optional)"'
            }
        }
    }
}
