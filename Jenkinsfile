pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Cloning repository...'
            }
        }

        stage('Build') {
            steps {
                echo 'Building backend Docker image...'
                sh 'docker build -t lab6-backend ./backend'
            }
        }

        stage('Run Nginx') {
            steps {
                echo 'Pulling nginx image...'
                sh 'docker pull nginx'
            }
        }
    }
}
