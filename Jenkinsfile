pipeline {
    agent any
    
    environment {
        PATH = "C:\\Program Files\\Java\\jdk-21\\bin;${env.PATH}"
        PHP_PATH = "E:\\xampp\\php"
        COMPOSER_HOME = "C:\\Users\\Administrator\\AppData\\Roaming\\Composer"
        PROJECT_DIR = "E:\\PRAN-RFL\\practise\\CI-CD"
    }

    stages {
        stage('Checkout') {
            steps {
                // Checkout the code from the Git repository
                dir("${PROJECT_DIR}") {
                    git branch: 'main', url: 'https://github.com/sehirulislamrehi/ci-cd'
                }
            }
        }
        
        stage('Install Dependencies') {
            steps {
                // Install PHP dependencies using Composer
                dir("${PROJECT_DIR}") {
                    bat "${PHP_PATH}\\php.exe ${COMPOSER_HOME}\\composer.phar install --no-dev"
                }
            }
        }

        stage('Run Tests') {
            steps {
                // Run PHPUnit tests
                dir("${PROJECT_DIR}") {
                    bat "${PHP_PATH}\\php.exe vendor\\bin\\phpunit"
                }
            }
        }

        stage('Build') {
            steps {
                // Prepare the project for deployment (e.g., generate application key)
                dir("${PROJECT_DIR}") {
                    bat "copy .env.example .env"
                    bat "${PHP_PATH}\\php.exe artisan key:generate"
                }
            }
        }

        stage('Deploy') {
            steps {
                // Deploy the project to the server (replace with your deployment steps)
                // Example: bat "${PHP_PATH}\\php.exe artisan migrate --force"
            }
        }
    }

    post {
        success {
            sh 'cd "E:\PRAN-RFL\practise\CI-CD" '                                
            sh 'ni hello.txt'                                
        }
        always {
            // Clean up steps
            dir("${PROJECT_DIR}") {
                bat "del /Q /S /F .env"
            }
        }
    }
}
