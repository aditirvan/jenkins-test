pipeline {
    agent any

    stages {
        stage('Pertama') {
            steps {
                echo 'Building..'
                sh 'ls'
                sh 'pwd'
                sh 'ssh web-server ls /var/www/html'
            }
        }
        
    }
}