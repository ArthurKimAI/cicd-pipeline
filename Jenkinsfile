pipeline {
  agent any
  stages {
    stage('first') {
      steps {
        sh 'npm install'
      }
    }

    stage('second') {
      steps {
        sh './build.sh'
      }
    }

  }
  environment {
    cicd = 'first'
  }
}