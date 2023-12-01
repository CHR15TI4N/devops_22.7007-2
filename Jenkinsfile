pipeline{
    
    agent any

    stages{
        stage('test'){
            steps{
                sh '''
                npm install
                npm test
                '''
            }
        }
        stage('build'){
            steps{
                sh'''
                docker-compose build
                '''
            }
        }
    }
}