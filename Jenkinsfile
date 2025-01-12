pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/ArthurKimAI/cicd-pipeline.git'
            }
        }

        stage('Build Application') {
            steps {
                sh './build.sh'
            }
        }

        stage('Tests') {
            steps {
                sh './test.sh'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh "docker build . -t ${arthurkimmel}/${mybuildimage}:${env.BUILD_NUMBER}"
            }
        }
    }
}
