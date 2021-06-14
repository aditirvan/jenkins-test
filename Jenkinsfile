pipeline {
    agent any

    stages {
        stage('Preparing') {
            steps {
                echo 'Building..'
                sh 'ls'
                sh 'pwd'
            }
        }
        stage('Copying') {
            steps {
                echo 'Copying files to web-server'
                sh 'rsync -r . ec2-user@web-server:/var/www/html'
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