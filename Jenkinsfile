pipeline {
    agent any

    stages {

        stage('Checkout Code') {
            steps {
                git 'https://github.com/rahularkala/devops-demo-app.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t devops-demo .'
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker run -d -p 3000:3000 devops-demo'
            }
        }
    }
}