pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Deploy') {
            steps {
                // index.html을 Nginx 경로로 복사
                sh 'cp index.html /var/www/html/'
                echo '배포 완료!'
            }
        }
    }
}