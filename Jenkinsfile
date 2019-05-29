pipeline {
    agent any
    
    tools {nodejs "node"}

    stages {
        stage('Build') {
            steps {
                bat 'npm install'
            }
        }
        stage('Test') {
            steps {
                //bat 'npm test'
                echo 'Testing'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}