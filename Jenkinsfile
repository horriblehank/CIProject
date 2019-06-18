pipeline {
    agent any
    
    tools {nodejs "node"}

    stages {
         stage('install dependencies') {
            steps {
                sh 'npm install'
            }
        }
        stage('Build dist files') {
            steps {
                sh 'npm run build'
            }
        }
        stage('Run unit tests') {
            steps {
                sh 'npm run test'
            }
        }
        stage('deploy application') {
            steps {
                sh 'npm run deploy'
            }
        }
    }
}