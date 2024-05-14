pipeline {
    agent any
    
    environment {
        PATH = "C:\\Program Files\\Java\\jdk-21\\bin;${env.PATH}"
        PHP_PATH = "E:\\xampp\\php"
        COMPOSER_HOME = "C:\\Users\\Administrator\\AppData\\Roaming\\Composer"
        PROJECT_DIR = "E:\\PRAN-RFL\\practise\\CI-CD"
        JENKINS_DIR = "C:\ProgramData\Jenkins\.jenkins\workspace\LaravelTest"
    }

    stage("For Main") {
        when {
            branch 'main'
        }
        steps {
            sshagent(credentials: ['LaravelTest']) {
                sh '''
                    ssh -o StrictHostKeyChecking=no root@172.17.2.162 whoami
                '''
            }
            
        }
        
    }

}
