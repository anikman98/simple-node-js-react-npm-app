pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                echo "Installing dependencies..."
                bat 'npm install' 
            }
        }
        stage('Test'){
            steps {
                echo "Starting tests..."
                bat './jenkins/scripts/test.sh'
            }
        }
    }
}