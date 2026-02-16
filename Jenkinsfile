pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Checking out source code...'
            }
        }

        stage('Build') {
            steps {
                echo 'Compiling Java program...'
                sh 'javac Hello.java'
            }
        }

        stage('Test') {
            steps {
                echo 'Running Java program...'
                sh 'java Hello'
            }
        }
    }

    post {
        success {
            echo 'Build Successful!'
        }
        failure {
            echo 'Build Failed!'
        }
    }
}
