pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo "Build step for static website"
                bat 'dir'
            }
        }

        stage('Test') {
            steps {
                echo "Checking index.html"
                bat 'dir index.html'
            }
        }

        stage('Deploy') {
            steps {
                echo "Website deployed to Jenkins workspace"
            }
        }
    }
}
