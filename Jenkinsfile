pipeline{
    
    agent any

    stages{
        stage('Build TADS'){
            steps{
                sh '''
                docker --version
                java --version
                docker info
                '''
            }
        }
    }
}