pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                echo "Building ..."
            }
            post{
                success{
                    mail to: "tomledeakin@gmail.com",
                    subject: "Build Status Email",
                    body: "Build log attached!"
                }
            }
        }
        stage('Test'){
            steps{
                echo "Testing ..."
            }
        }
        stage('Deploy'){
            steps{
                echo "Deploying ..."
            }
        }
    }
}
