pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                echo "Cloning the repository..."
                git 'https://github.com/SnehalGuruphale/exp5_Jenkins.git'
            }
        }

        stage('Build') {
            steps {
                echo "Build step for static website - nothing to compile"
            }
        }

        stage('Test') {
            steps {
                echo "Testing if index.html exists"
                bat 'dir index.html'
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploying website to Jenkins workspace"
            }
        }
    }
}
