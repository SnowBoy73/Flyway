pipeline {
    agent any
    stages {
        stage("Deliver database") {
            steps {
                sh "docker-compose up -d app-database"
                sh "docker-compose up flyway"
            }
        }
    }
}