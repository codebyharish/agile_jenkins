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
                bat 'javac Hello.java'
                bat 'java Hello'

            }
        }

        stage('Test') {
            steps {
                echo 'Running Java program...'
                bat 'javac Hello.java'
                bat 'java Hello'

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
