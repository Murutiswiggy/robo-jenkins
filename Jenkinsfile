
pipeline {
    agent {
        node {
            label 'ROBO'
        }
    }

    environment {
        CC = credentials('key')
    }

    stages {
        stage('Build') {
            steps {
                sh '''
                    echo 'Building..'
                    echo 'CC is configured'
                '''
            }
        }

        stage('Test') {
            steps {
                sh '''
                    echo 'Testing..'
                '''
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                    echo 'Deploying..'
                '''
            }
        }
    }

    post {
        always {
            echo 'I will always say Hello again!'
        }

        success {
            echo 'I will success say Hello again!'
        }

        failure {
            echo 'I will failure say Hello again!'
        }
    }
}
