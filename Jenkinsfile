pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                bat 'python -m py_compile factorial.py'
            }
        }

        stage('Test') {
            steps {
                bat 'python factorial.py'
            }
        }
    }
}