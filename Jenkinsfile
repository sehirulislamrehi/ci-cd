pipeline {
    agent any
    stages {
        stage('Debug') {
            steps {
                script {
                    echo "Environment: ${env}"
                    sh 'which ssh-agent'
                }
            }
        }
    }
}
