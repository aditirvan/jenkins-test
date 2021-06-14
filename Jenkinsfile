pipeline {
    agent any

    stages {
        stage('Pertama') {
            steps {
                echo 'Building..'
                sh 'ls'
                sh 'pwd'
                sh 'rsync -r . root@web-server:/var/www/html'
            }
        }
        
    }
}