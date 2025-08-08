pipeline {
    agent any

    triggers {
        // Trigger build when a push event is received from GitHub webhook
        githubPush()

         // Poll GitHub every 1 minute for changes
        pollSCM('* * * * *')
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

            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                // Example test command

            }
        }
stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Example deploy command
        
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
