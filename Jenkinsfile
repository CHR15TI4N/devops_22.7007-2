pipeline {
    agent agent

    stages {
        stage('Build TADS') {
            steps {
                sh '''

                docker --version
                docker-compose --version
                java --version
                jenkins --version
                
                '''
            }
        }
    }
}