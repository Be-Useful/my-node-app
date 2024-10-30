pipeline {
    agent any

    stages {
        stage('Check Node Version') {
            steps {
                script {
                    // Check if Node.js is installed
                    def nodeVersion = sh(script: 'node -v', returnStdout: true).trim()
                    echo "Node.js version: ${nodeVersion}"
                }
            }
        }
    }
}
