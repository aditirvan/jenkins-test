pipeline {
    agent any

    stages {
        stage('Pertama') {
            steps {
                echo 'Building..'
                sh 'ls'
                sh 'pwd'    
                sh 'rsync -r . webdev:/var/www/html/adhithia/'
                sh 'ssh webdev ls /var/www/html/adhithia/'
            }
        }
        
    }
}