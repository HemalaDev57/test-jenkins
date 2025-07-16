pipeline {
    agent any

    triggers {
        cron('H * * * *') // Every hour at a hashed minute
    }

    stages {
        stage('Hourly Task') {
            steps {
                echo "Running hourly job at: ${new Date()}"
                sleep 20
            }
        }
    }
}
