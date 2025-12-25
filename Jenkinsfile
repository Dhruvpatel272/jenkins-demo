pipeline {
    agent any

    stages {
        stage('Run App Script') {
            steps {
                sh 'chmod +x app.sh'
                sh './app.sh'
            }
        }
    }
}
