pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
                sh 'docker build -t lucky-app .'
            }
        }

        stage('Run Docker Container') {
            steps {
                sh 'docker run --rm lucky-app'
            }
        }
    }
}
