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

    stage('third') {
      steps {
        sh './test.sh'
      }
    }

  }
  environment {
    cicd = 'first'
  }
}