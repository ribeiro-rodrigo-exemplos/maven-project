pipeline{
    agent any 
    stages{
        stage('Build'){
            steps{
                sh 'mvn clean package'
                sh "docker image build . -t tomcatwebapp:${env.BUILD_ID}"
            }
        }
    }
}