pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/Dhruvpatel272/jenkins-demo.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh ''docker --verion'
                sh ''docker build -t jenkins-demo:1.0 ."            
            }
        }
        stage ('Run Docker container'){
            steps{
                sh 'docker run --rm jenkins-demo:1.0"
            }
        }
    }
}
