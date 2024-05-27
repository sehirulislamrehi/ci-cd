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
                    echo "PATH: ${env.PATH}"
                    echo "PHP_PATH: ${env.PHP_PATH}"
                    echo "COMPOSER_HOME: ${env.COMPOSER_HOME}"
                    echo "PROJECT_DIR: ${env.PROJECT_DIR}"
                    echo "JENKINS_DIR: ${env.JENKINS_DIR}"

                    // Check if ssh-agent is available
                    sh 'ssh-agent -v'
                }
            }
        }
    }
}
