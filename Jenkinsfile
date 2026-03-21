pipeline {
    agent any

    stages {

        stage('Install Dependencies') {
            steps {
                sh 'docker run --rm -v ${WORKSPACE}:/app -w /app node:18 npm install'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t devops-demo ${WORKSPACE}'
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker run -d -p 3000:3000 devops-demo'
            }
        }
    }
}