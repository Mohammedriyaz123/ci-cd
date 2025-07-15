pipeline {
    agent any

    stages {
        stage('Clone Code') {
            steps {
                git 'https://github.com/Mohammedriyaz123/ci-cd'
            }
        }

        stage('Build') {
            steps {
                echo 'No build step needed for static HTML.'
            }
        }

        stage('Test') {
            steps {
                echo 'Skipping tests for static HTML.'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying index.html to /var/www/html...'
                sh 'sudo cp index.html /var/www/html/index.html'
            }
        }
    }
}
