pipeline {
    agent any

    stages {
        stage('Preparing') {
            steps {
                echo 'Building..'
                sh 'ls'
                sh 'pwd'
                echo 'Stopping apache'
                sh 'ssh root@13.250.3.75 "systemctl stop httpd"'
            }
        }
        stage('Copying') {
            steps {
                echo 'Copying files to 13.250.3.75'
                sh 'rsync -r . root@13.250.3.75:/var/www/html'
                sh 'ssh root@13.250.3.75 "systemctl start httpd"'
            }
        }
        stage('Done') {
            steps {
                echo 'Completed'
                echo 'Send notification to developer'
            }
        }
    }
}