pipeline {
    agent {
        node{
            label 'ROBO'
        }
    }

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
               script{
                 sh """
                    echo 'Testing..'
                """
               }
            }
        }

        stage('Deploy') {
            steps {
                script{
                    sh """
                    echo 'Deploying..'
                """
                }
               
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