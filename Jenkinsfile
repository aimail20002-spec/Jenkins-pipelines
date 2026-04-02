pipeline {
    agent any
    stages {
        stage('Install Dependencies') {
            steps {
                echo '📦 Installing npm dependencies...'
                bat 'npm install'
            }
        }
        stage('Build') {
            steps {
                echo '🏗️ Building project...'
                bat 'npm run build'
            }
        }
        stage('Test') {
            steps {
                echo '🧪 Running tests...'
                bat 'npm test'
            }
        }
        stage('Deploy') {
            steps {
                echo '🚀 Deploying project...'
                bat 'echo Deploy step here'
            }
        }
    }
    post {
        always {
            echo '🔔 Pipeline finished.'
        }
    }
}
