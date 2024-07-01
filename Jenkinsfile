pipeline {
    agent any

    stages {
        stage('Echo') {
            steps {
                echo 'Hello World!'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}
