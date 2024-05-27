pipeline {
    agent any
    
    environment {
        PATH = "C:\\Program Files\\Java\\jdk-21\\bin;${env.PATH}"
        PHP_PATH = "E:\\xampp\\php"
        COMPOSER_HOME = "C:\\Users\\Administrator\\AppData\\Roaming\\Composer"
        PROJECT_DIR = "E:\\PRAN-RFL\\practise\\CI-CD"
        JENKINS_DIR = "C:\\ProgramData\\Jenkins\\.jenkins\\workspace\\LaravelTest"
        SSH_CREDENTIALS = credentials('crm-test')
    }

    stages {
        stage("For Main") {
            steps {
                script {
                    sshagent(['crm-test']) {
                        sh '''
                            ssh -o StrictHostKeyChecking=no root@172.17.2.162 whoami
                        '''
                    }
                }
            }
        }
    }
}
