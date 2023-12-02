pipeline{
    
    agent any

    stages{
        stage('start NodeGoat'){
            steps{
                sh '''
                npm install
                '''
            }
        }
        stage('test'){
            steps{
                sh'''
                npm test
                '''
            }
        }
        stage('docker building'){
            steps{
                sh'''
                docker build
                '''
            }
        }
        stage('rodar o projeto'){
            steps{
                sh'''
                docker compose up
                '''
            }
        }
    }
}