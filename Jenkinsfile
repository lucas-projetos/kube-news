pipeline{
    agent any

    stages{
        stage('Build docker image'){
            steps{
                script{
                    dockerapp = docker.build("oliver4303/kube-news:${env.BUILD_ID}", '-f ./src/Dockerfile ./src')
                }
            }
        }
    }
}