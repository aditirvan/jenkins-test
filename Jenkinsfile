pipeline {
    agent any

    stages {
        stage('Pertama') {
            steps {
                echo 'Building..'
                sh 'ls'
                sh 'ssh -i "test-adhithia.pem" ec2-user@ec2-18-223-186-17.us-east-2.compute.amazonaws.com'
            }
        }
        
    }
}