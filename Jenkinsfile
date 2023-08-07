pipeline{
    agent any
    stages {
        stage('Verify verssion'){
            steps {
                sh 'docker run --rm flyway/flyway:8.5.1 version'
            }
        }
    }
}