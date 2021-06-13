pipeline {
    agent any

    stages {
        stage('Pertama') {
            steps {
                echo 'Building..'
                sh 'ls'
                sh 'scp -i test-adhithia.pem . root@18.223.186.17:/var/www/html/adhithia/'
            }
        }
        
    }
}