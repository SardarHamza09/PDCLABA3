pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps { checkout scm }
        }
        stage('Build') {
            steps { sh 'python3 hello.py' }
        }
        stage('Test') {
            steps { sh 'python3 -m py_compile hello.py' }
        }
    }
}
