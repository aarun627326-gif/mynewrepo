pipeline {
    agent any  // Runs on any available Jenkins agent

    stages {
        stage('Checkout Code') {
            steps {
                // Pull code from your GitHub repository
                git branch: 'master', url: 'https://github.com/aarun627326-gif/mynewrepo.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the application...'
                // Example: if it's a Java app
                // sh 'mvn clean package'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                // Example: if you have test scripts
                // sh 'mvn test'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                // Example: run deployment commands here
            }
        }
    }

    post {
        success {
            echo 'Pipeline executed successfully!'
        }
        failure {
            echo 'Pipeline failed. Check the logs.'
        }
    }
}
