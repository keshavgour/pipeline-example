pipeline {

    agent any
    stages{

        stage("compile"){

            steps{
                bat 'javac Demo.java'
            }
        }

        stage("run"){

            steps{
                bat 'java Demo'
            }
        }
    }
        post{

            always {
                
                bat 'echo "always"'
            }

            success {

                bat 'echo "Success"'
            }

            failure {

                bat 'echo "failure"'
                
            }
        }

    }
