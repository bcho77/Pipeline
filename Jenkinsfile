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
                // Build your application (e.g., compile, package)
                //sh 'mvn clean package' // Adjust this command based on your project's build process
              echo "i love you"
            }
        }
        
        stage('Deploy') {
            steps {
                // Deploy your application (e.g., copy files, deploy to a server)
                //sh 'scp target/your-app.war user@your-server:/path/to/deployment/directory' // Example SCP command
              echo "i love you"
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
