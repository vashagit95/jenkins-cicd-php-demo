pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                // Get code from a GitHub repository
                git url: 'https://github.com/vashagit95/jenkins-cicd-php-demo.git', branch: 'main',
                 credentialsId: 'vashagit95'
            }
        }
    }
}