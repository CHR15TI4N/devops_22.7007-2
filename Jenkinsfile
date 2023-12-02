pipeline {
    agent any

    tools {nodejs 'node'}

    stages {
        stage('INSTALL'){
            steps{
                sh '''
                npm install
                '''
            }
        }
//         stage('test'){
//             steps{
//                 sh 'npm test'
//             }
//         }
//         stage('build') {
//             steps {
//                 sh 'docker build -t trabalho .' 
//             }
//         }
//          stage('up') {
//             steps {
//                 sh 'docker compose up'  
//             }
//         }
    }
}