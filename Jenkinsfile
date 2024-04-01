pipeline {
    agent any

    tools{
        maven 'Maven'
    }
    
    stages {
        stage("Checkout") {
            steps {
                git branch: 'master', url: 'https://github.com/shindenikhil659/CI-CD-Pipeline.git'
            }
        }
        
        stage("Build") {
            steps {
                bat 'mvn clean'
            }
        }
        
        stage("Test") {
            steps {
                bat 'mvn test'
            }
        }
        
        stage("Deploy") {
            steps {
                echo 'Deployed Successfully'
            }
        }
    }
}
