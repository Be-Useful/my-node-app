pipeline {
    agent any

    stages {
        stage('Check Node Version') {
            steps {
                script {
                    try {
                        // Check if Node.js is installed
                        def nodeVersion = sh(script: 'node -v', returnStdout: true).trim()
                        echo "Node.js version: ${nodeVersion}"
                    } catch (Exception e) {
                        echo "Node.js is not installed. Please install Node.js before running this pipeline."
                        error "Node.js not found"
                    }
                }
            }
        }
    }
}
