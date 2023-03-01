pipeline{
    agent any

    stages{
        stage('Checkout'){
            steps {
                git branch: 'master', url: 'https://github.com/Khady199/Jenkins.git'
                
            }
        }
        stage ('build'){
            steps{
                bat 'npm install'
            }
        }
        stage('Test'){
            steps{
                bat 'npm run test'
            }
        }
        satge('deploy'){
            steps{
                bat 'npm run start'
            }
        }
    }
}