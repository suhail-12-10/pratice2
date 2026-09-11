pipeline {
    agent any

    stages {

        stage('checkout') {
            steps {
                Checkout scm
            }
        }

        stage('Test') {
            steps {
                sh 'echo Running tests'
            }
        }

        stage('Build') {
            steps {
                sh 'echo Running build'
            }
        }
    }

    post {
        success {
            echo 'Pipeline successful'
        }

        failure {
            echo 'Pipeline failed'
        }
    }
}
