pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
                sh 'sudo docker build -t lucky-app .'
            }
        }

        stage('Run Docker Container') {
            steps {
                sh 'sudo docker run --rm lucky-app'
            }
        }
    }
}
