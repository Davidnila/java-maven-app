pipeline {
    agent any

    environment {
        BRANCH_NAME = env.GIT_BRANCH ?: 'main' // Default ke 'main' jika GIT_BRANCH tidak ada
    }

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Test') {
            steps {
                script {
                    echo "Testing aplikasi di branch ${BRANCH_NAME}..."
                }
            }
        }

        stage('Build') {
            steps {
                script {
                    echo "Build aplikasi..."
                }
            }
        }

        stage('Deploy') {
            steps {
                script {
                    echo "Deploy aplikasi..."
                }
            }
        }
    }
}
