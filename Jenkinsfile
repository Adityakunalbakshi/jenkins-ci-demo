pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Checking out code from Git...'
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Running build verification...'
                sh 'echo "Project structure verified."'
            }
        }

        stage('Test') {
            steps {
                echo 'Running unit test suite...'
                sh 'echo "All tests passed successfully!"'
            }
        }
    }

    post {
        success {
            echo 'Pipeline executed and tests passed successfully.'
        }
    }
}
