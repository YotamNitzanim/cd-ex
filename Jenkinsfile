pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'ls -lah'
                sh 'ls'
            }
        }
        stage('test') {
            steps {
                sh 'pwd'
            }
        }
        stage('deploy') {
            steps {
                sh 'ssh ubuntu@ec2-18-177-121-218.ap-northeast-1.compute.amazonaws.com docker run --name docker-guide -d -p 81:80 docker/getting-started'
            }
        }
        
    }
}
