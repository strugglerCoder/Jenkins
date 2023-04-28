pipeline{
    agent any

    stages{
        stage("Git Checkout"){
            steps{
                git credentialsId: 'git', url: 'https://github.com/strugglerCoder/Jenkins.git'
                echo "Git fetch successfully..."
            }
        }

        stage("Build"){
            steps{
                script{

                }
            }
        }
        
        stage("Deploy"){
            steps{
                script{

                }
            }
        }
    }
}