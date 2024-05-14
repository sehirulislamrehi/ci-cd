pipeline {
    agent any
    
    environment {
        PATH = "C:\\Program Files\\Java\\jdk-21\\bin;${env.PATH}"
        PHP_PATH = "E:\\xampp\\php"
        COMPOSER_HOME = "C:\\Users\\Administrator\\AppData\\Roaming\\Composer"
        PROJECT_DIR = "E:\\PRAN-RFL\\practise\\CI-CD"
        JENKINS_DIR = "C:\\ProgramData\\Jenkins\\.jenkins\\workspace\\LaravelTest"
    }

    stages {
        stage("For Main") {
            steps {
                script {
                    sshagent(credentials: ['crm-test']) {
                        sh '''
                            ssh -o StrictHostKeyChecking=no root@172.17.2.162 whoami
                        '''
                    }
                    dir("${JENKINS_DIR}") {
                        fileOperations([fileCopyOperation(excludes: '', flattenFiles: true, includes: '.env', targetLocation: "${WORKSPACE}")])
                    }
                }
            }
        }
    }
}
