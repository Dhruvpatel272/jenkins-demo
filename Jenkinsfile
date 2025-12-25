pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        
        stage('Run App') {
            steps {
                sh 'ls -la'
                sh 'chmod +x app.sh'
                sh 'sh app.sh'
            }
        }
    }
}
