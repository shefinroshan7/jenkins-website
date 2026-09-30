pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Getting website code from GitHub...'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying website...'
                sh 'sudo cp index.html /var/www/html/index.html'
            }
        }

        stage('Verify') {
            steps {
                sh 'curl -I http://localhost'
            }
        }
    }
}