pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'docker build -t flask-app .'
            }
        }

        stage('Test') {
            steps {
                sh 'echo "Skipping tests for now"'
            }
        }

        stage('Deploy') {
            steps {
                sh 'docker run -d -p 5000:5000 flask-app'
            }
        }
    }
}
