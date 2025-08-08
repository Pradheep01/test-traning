pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/Pradheep01/test-traning.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Building the project...'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }
    }
}
