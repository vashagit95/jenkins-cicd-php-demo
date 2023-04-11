pipeline {
    agent any
    environtment{
        staging_server="54.254.122.239"
    }
    stages {
        stage('Build') {
            steps {
                // Get code from a GitHub repository
                sh 'scp ${WORKSPACE}* ubuntu@$staging_server}:/var/www/html/',
                 credentialsId: 'vashagit95'
            }
        }
    }
}