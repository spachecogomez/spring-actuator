pipeline {
    agent {
        docker {
            image 'maven:3.3.3'
            args '-v /var/run/docker.sock:/var/run/docker.sock'
        }
    }
    stages {
        stage('build') {
            steps {
                sh 'mvn clean install'
            }
        }
    }
}