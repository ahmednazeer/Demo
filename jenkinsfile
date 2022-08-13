pipeline{
    agent any
    stages{
       stage('Checkout') {
          steps {
           git credentialsId: '	github-info', 
           url: 'https://github.com/ahmednazeer/Demo/', 
           branch: 'dev'
           },
           stage('Build'){
             steps{
                bat "dotnet build E:\Problem Solving\Demo\Demo\Demo.API\\Demo.API.csproj --configuration Release"
              }
           }
    }
    environment {
        dotnet ='C:\\Program Files (x86)\\dotnet\\'
        }
        
    triggers {
        pollSCM 'H * * * *'
    }
 }
