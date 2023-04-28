pipeline{
    agent any

    stages{

        stage('Git Checkout'){
            steps{
                git credentialsId: 'git', url: 'https://github.com/strugglerCoder/Jenkins.git'
                echo "Git fetch successfully..."
            }
        }

        stage('Build'){
            steps{
                script{
                    echo "Building..."
                }
            }
        }
        
        stage('Deploy'){
            steps{
                script{
                    echo "Deploying..."
                }
            }
        }
    }
}