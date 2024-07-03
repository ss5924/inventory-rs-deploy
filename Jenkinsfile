pipeline {
    agent any

    environment {
        DOCKER_REGISTRY = "192.168.0.37:5000"
        DEPLOY_FILE = "docker-compose.yml"
    }

    stages {
        stage('checkout') {
            steps {
                checkout scm
            }
        }

        stage('Deploy with Docker Compose') {
            steps {
                script {
                    withEnv(["DOCKER_REGISTRY=${DOCKER_REGISTRY}"]) {
                        sh 'docker-compose -f ${DEPLOY_FILE} down'
                        sh 'docker-compose -f ${DEPLOY_FILE} up -d'
                    }
                }
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
        always {
            script {
                sh 'docker-compose -f ${DEPLOY_FILE} logs'
            }
        }
    }
}
