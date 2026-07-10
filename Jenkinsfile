pipeline {
    agent any

    environment {
        VERCEL_TOKEN = credentials('vercel_token')
    }

    stages {
        stage ('install') {
            steps{
                bat 'npm install'
            }
        

        }
        
        stage ('test') {
            steps{
                bat 'no test script'
            }
        

        }
        
        stage ('bild') {
            steps{
                bat 'npm run build'

            }
        

        }

        stage ('deploy') {
            steps{
                bat 'npx vercel --prod --yes 
                --token=%vercel_token%'
            }
        

        }
    }
}