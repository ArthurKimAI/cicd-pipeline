pipeline {
  agent any
  stages {
    stage('first') {
      steps {
        sh 'npm install'
      }
    }

  }
  environment {
    cicd = 'first'
  }
}