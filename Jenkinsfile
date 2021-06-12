pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                'ssh webdev-vaf df -h'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}