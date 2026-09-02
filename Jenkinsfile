pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Checking out Fibonacci project'
                checkout scm
            }
        }

        stage('Test Python') {
            steps {
                bat 'python --version'
            }
        }

        stage('Run Fibonacci') {
            steps {
                bat 'echo 10 | python fibonacci.py'
            }
        }

        stage('Complete') {
            steps {
                echo 'Fibonacci Pipeline Completed Successfully'
            }
        }
    }
}