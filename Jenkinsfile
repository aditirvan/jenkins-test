pipeline {
    agent any

    stages {
        stage('Pertama') {
            steps {
                echo 'Building..'
                sh 'ls'
                sh 'pwd'    
                sh 'ssh webdev ls /var/www/html'
            }
        }
        
    }
}