pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/Dhruvpatel272/jenkins-demo.git'
            }
        }

        stage('Check Docker') {
            steps {
                sh 'docker --version'
            }
        }

        stage('Run App Script') {
            steps {
                sh 'chmod +x app.sh'
                sh './app.sh'
            }
        }
    }
}
