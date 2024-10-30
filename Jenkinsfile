pipeline {
    agent any

    tools {
        nodejs 'NodeJS01' // Ensure this matches the name you provided in Jenkins
    }

    stages {
        stage('Checkout Code') {
            steps {
                // Checkout the code from GitHub
                git 'https://github.com/Be-Useful/my-node-app.git' // Replace with your repository URL
            }
        }

        stage('Check Node Version') {
            steps {
                bat 'node -v' // Use bat instead of sh for Windows
            }
        }

        stage('Install Dependencies') {
            steps {
                bat 'npm install' // Install npm dependencies
            }
        }

        stage('Run Application') {
            steps {
                bat 'npm start' // Start the Node.js application
            }
        }
    }
}
