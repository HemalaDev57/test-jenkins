pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                sleep 10
            }
        }
        stage('Test') {
            steps {
                script {
                    echo 'Running tests...'
                    sleep 5
                    // Mark build as UNSTABLE intentionally
                    currentBuild.result = 'UNSTABLE'
                }
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                sleep 10
            }
        }
    }
}
