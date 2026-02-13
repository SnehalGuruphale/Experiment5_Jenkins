pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo "Build step"
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
                echo "Publishing HTML report in Jenkins"
                publishHTML([
                    reportDir: '.',
                    reportFiles: 'index.html',
                    reportName: 'My Website Output'
                ])
            }
        }
    }
}
