pipeline {
    agent any // You can specify a specific agent or label here

    stages {
        stage('Checkout') {
            steps {
                // Checkout the code from a Git repository
                script {
                    git 'https://github.com/bcho77/Pipeline.git'
                }
            }
        }
        
        stage('Build') {
            steps {
              echo 'i love you'
            }
        }
        
        stage('Deploy') {
            steps {
                
              echo 'i love you' 
            }
        }
    }
    
    post {
        success {
            echo 'Pipeline succeeded! Application deployed.'
        }
        failure {
            echo 'Pipeline failed. Check the build and deployment logs.'
        }
    }
}
