pipeline{
    agent any
    stages{
       stage('Checkout') {
           echo('checkout')
          steps {
           git credentialsId: '	github-info', 
           url: 'https://github.com/ahmednazeer/Demo/', 
           branch: 'dev'
           },
       stage('Build'){
         echo('Build')
       }
    }
    
 }
