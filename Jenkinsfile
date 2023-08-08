pipeline{
    agent {
        docker {
            image 'boxfuse/flyway:9'
            args '-v ./db/migration:/flyway/sql --entrypoint=\'\''
        }
    }
    stages {
        stage('Verify verssion'){
            steps {
                sh 'docker run --rm flyway/flyway:9 version'
            }
        }
    }
}