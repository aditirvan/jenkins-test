pipeline {
    agent any

    stages {
        stage('Pertama') {
            steps {
                echo 'Building..'
                sh 'ls'
                sh 'pwd'
                sh 'ssh webdev mkdir -p /home/valbury/adhithia'
                sh 'ssh webdev ls /home/valbury/'
                sh 'rsync -r . webdev:/home/valbury/adhithia/'
                sh 'ssh webdev ls /home/valbury/adhithia/'
            }
        }
        
    }
}