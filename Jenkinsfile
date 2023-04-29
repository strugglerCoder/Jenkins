pipeline{
    agent any

    stages{

        stage('Git Checkout'){
            steps{
                git credentialsId: 'git', url: 'https://github.com/strugglerCoder/Jenkins.git'
                echo "Git fetch successfully..."
            }
        }

        stage('Test'){
            steps{
                script{
                    echo "Testing..."
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

    post{
        success{
            emailext body: 'below Build Success ', recipientProviders: [developers()], subject: 'Build Success', to: 'holeajinkya118@gmail.com'
        }
    }
}