pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                // Clone the repository
                git branch: 'master', url: 'https://github.com/your-username/jenkins-ci-cd-demo.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                // Install project dependencies
                sh 'npm install'
            }
        }

        stage('Run Tests') {
            steps {
                // Run tests
                sh 'npm test'
            }
        }

        stage('Build') {
            steps {
                // Build the project (if applicable)
                sh 'echo "Building the project..."'
            }
        }

        stage('Deploy') {
            steps {
                // Deploy application (this can vary based on your environment)
                sh 'echo "Deploying the project..."'
            }
        }
    }

    post {
        success {
            echo 'Pipeline executed successfully.'
        }
        failure {
            echo 'Pipeline failed.'
        }
    }
}

