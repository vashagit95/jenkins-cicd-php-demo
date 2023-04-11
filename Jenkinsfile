pipeline {
    agent any
    environment{
        staging_server="54.254.122.239"
    }
    stages {
        stage('Deploy to Remote') {
            steps {
                // Get code from a GitHub repository
                sh 'scp ${WORKSPACE}/* ubuntu@${staging_server}:/var/www/html/'
            }
        }
    }
}