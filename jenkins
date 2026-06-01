pipeline{
    agent any
    stages{
        stage('Check Java Version'){
            steps{
                bat 'java -version'
                bat 'javac -version'
            }

        }
        stage('Compile Java Code'){
            steps{
                bat 'javac text_file.java'

            }
        }
        stage('Run Java Code'){
            steps{
                bat 'java text_file'
            }
        }
        
        
    }
    post{
        success{
            echo 'Build and execution successful!'
        }
        failure{
            echo 'Build or execution failed.'
        }
    }
}