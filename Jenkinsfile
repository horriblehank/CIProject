pipeline {
    agent any
    
    tools {nodejs "node"}



    stages {

        stage('Install') {
            steps {
                sh 'npm install'
            }
        }

        stage('Build') {
            steps {
                sh 'npm run build'
            }
        }

        

/*        stage('Deploy') {
            steps {
                sh 'az storage blob upload-batch -s /var/lib/jenkins/workspace/Hypertime_master/hypertime-frontend/build -d /$web --connection-string="DefaultEndpointsProtocol=https;AccountName=hypertimehenrik;AccountKey=IpfrB5TP7FFm7K+rcRg+B6vE6qJIW+vL7HYl9MU2pZrAXqQdYzClMlJCR3htcbqcMofApx+b60UEbD1R0LRIPA==;EndpointSuffix=core.windows.net"'
            }*/
        }
        


}