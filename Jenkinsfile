pipeline {
    agent any
    stages {
        stage('Lint') {
            steps {
                sh 'tidy -q -e blue/*.html'
                sh 'tidy -q -e green/*.html'
            }
        }
    }
}