pipeline {
    agent any
    
    tools {nodejs "node"}

    stages {
        stage('Build') {
            steps {
                bat 'npm install'
            }
        }        
        stage('Build Production files') {
                steps {
                    bat 'npm run build'
                }
            }        
        stage('Test') {
            steps {
                bat 'npm run test -- --coverage'
                //echo 'Testing'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}