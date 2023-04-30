pipeline{
    agent any

    stages{

        stage('Git Checkout'){
            steps{
                git credentialsId: 'git', url: 'https://github.com/strugglerCoder/Practice-Mode.git'
                echo "Git fetch successfully..."
            }
        }

        stage('Download Git Content'){
            steps{
                script{
                    sh 'git clone https://github.com/strugglerCoder/Practice-Mode.git'
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
            emailext body: 'below Build Success ', 
            recipientProviders: [developers()], 
            subject: 'Build Success', 
            to: 'ajshole@gmail.com'
        }
    }
}