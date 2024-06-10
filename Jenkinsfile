pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Checkout the code from the repository
                git branch: 'main', url: 'https://github.com/MohamedHammouda/JenkinsfileProject.git'
            }
        }
        
        stage('Build') {
            steps {
                // Run the build process
                sh 'echo "./build.sh"'
            }
        }
        
        stage('Test') {
            steps {
                // Run the tests
                sh 'echo "./test.sh"'
            }
        }
        
        stage('Deploy') {
            steps {
                // Deploy the application
                sh 'echo "./deploy.sh"'
            }
        }
    }
}
