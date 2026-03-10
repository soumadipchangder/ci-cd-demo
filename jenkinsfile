pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/soumadipchangder/ci-cd-demo'
            }
        }

        stage('Build') {
            steps {
                echo "Building application..."
            }
        }

        stage('Test') {
            steps {
                echo "Running tests..."
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                mkdir -p /Users/soumyadip/Desktop/deploy-demo
                cp index.html /Users/soumyadip/Desktop/deploy-demo/
                '''
            }
        }
    }
}
