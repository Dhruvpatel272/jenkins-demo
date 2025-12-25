pipeline {
  agent any

  stages {
    stage('Checkout') {
      steps {
        checkout scm
      }
    }

    stage('Build Docker Image') {
      steps {
        sh 'docker build -t jenkins-demo:latest .'
      }
    }

    stage('Run Container') {
      steps {
        sh '''
          docker rm -f jenkins-demo-container || true
          docker run -d --name jenkins-demo-container jenkins-demo:latest
        '''
      }
    }
  }
}
