pipeline {
    agent any

    stages {
        stage('Preparing') {
            steps {
                echo 'Building..'
                sh 'ls'
                sh 'pwd'
                echo 'Stopping apache'
                sh 'ssh root@web-server systemctl stop httpd'
            }
        }
        stage('Copying') {
            steps {
                echo 'Copying files to web-server'
                sh 'rsync -r . root@web-server:/var/www/html'
                sh 'ssh root@web-server systemctl start httpd'
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