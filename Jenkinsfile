pipeline {
    agent any
    stages{

        stage ("Git checkout"){
            steps{
              git url: 'https://github.com/jfneto7/jfneto-web.git', branch:'main'
            }
        }

        stage ("Test"){
            steps{
                sh 'which docker-compose'
            }
        }

        stage("Build"){
            steps{
                sh '/usr/bin/docker-compose up'
            }
        }

        stage("Deploy"){
            steps{
                sh 'echo "THE END "'
            }
        }
    }
}