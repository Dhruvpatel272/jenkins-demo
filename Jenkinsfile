pipeline {
    agent any

    stages {
        stage('Run App') {
            steps {
                sh 'ls -la'
                sh 'chmod +x app.sh'
                sh './app.sh'
            }
        }
    }
}
