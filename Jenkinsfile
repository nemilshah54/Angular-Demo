pipeline {
    agent any

    stages {
      
      
      stage('Install') {
            steps {
                bat 'npm i puppeteer' 
            }
        }
        
         
           stage('Compile') {
            steps {
                bat 'node_modules/.bin/ng build' 
            }
        }
      
       stage('Test') {
            steps {
                bat 'node_modules/.bin/ng test --browsers=Chrome --watch=false'
            }
        }
        
    }
}
