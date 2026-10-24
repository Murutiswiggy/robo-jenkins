pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script{
                    sh """
                        echo 'Building..'
                    """
                }
            }
        }
        stage('Test') {
            steps {
                   sh """
                        echo 'Testing..'
                    """
                 }

            }
        }
        stage('Deploy') {
            steps {
                 sh """
                     echo 'Deploying..'
               """
            
        }
    }
}