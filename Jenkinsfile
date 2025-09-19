pipeline {
    agent any

    parameters{
        choice(name: 'ENV', choices: ['DEV', 'QA', 'PROD'], description: 'Select the environment to deploy')
        string(name: 'Version', defaultValue: '1.0', description: 'Enter the version to deploy')
    }
    stages{
        stage('Build'){
            steps{
                echo "Building version ${params.Version} for environment ${params.ENV}..."
            }
           
        }
        stage('Test'){
            steps{
                echo "Testing....."
            }
        }
        stage('Deploy'){
            steps{
                echo "Deploying ${params.Version} to ${params.ENV}..."
            }
            
        }
    }   
 }