pipeline {
    agent any
    stages {
        stage('Lint') {
            steps {
                sh 'tidy -q -e blue/*.html'
                sh 'tidy -q -e green/*.html'
            }
        }
        stage('Build Image') {
            steps {
                sh 'blue/run_docker.sh'
                sh 'green/run_docker.sh'
            }
        }
    }
}