pipeline {
    agent any
    
    stages{
        stage('Checkout'){
            steps{
                echo "Checking the code"
            }
        }
        stage('Building'){
            steps{
            bat 'docker build -t myapp:latest .'
        }
    }
        stage('run container'){
            steps{
                bat 'docker run --name myapp myapp:latest'
            }
        }
    }
}
