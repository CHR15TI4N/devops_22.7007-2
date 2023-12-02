pipeline{

    agent any
       tools {nodejs 'node'}

    stages {
        stage('Start NodeGoat') {
            steps {
                sh '''
                npm install
                '''
            }
        }
        stage('Test NPM') {
            steps {
                sh '''
                npm test
                '''
            }
        }
        stage('Construindo Docker') {
            steps {
                sh '''
                docker-compose build
                '''
            }
        }

         stage('Testando Docker') {
            steps {
                echo 'Testing'
                sh '''
                npm install
                npm test
                '''
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy'
                sh '''
                docker-compose up
                '''
            }
        }
    }
}