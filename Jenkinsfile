pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building the Django project...'
                sh 'pip install -r requirements.txt'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'python manage.py test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                // Normally you would have deployment steps here
            }
        }
    }
}
