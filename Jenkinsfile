pipeline {
    agent any

    triggers {
        // Trigger build when a push event is received from GitHub webhook
        githubPush()
    }

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/Pradheep01/test-traning.git'
            }
        }
stage('Build') {
            steps {
                echo 'Running build...'
                // Example build command
              //  sh 'npm install'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                // Example test command
              //  sh 'npm test'
            }
        }
stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Example deploy command
             //   sh './deploy.sh'
            }
        }
    }

    post {
        success {
            echo ' Build and deployment completed.'
        }
        failure {
            echo ' Build or deployment failed.'
        }
    }
}
