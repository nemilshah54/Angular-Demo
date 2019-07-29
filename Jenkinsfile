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
                bat 'node_modules/.bin/ng test'
            }
        }
      
      stage('Deploy') {
            steps {
                bat 'node_modules/.bin/ng build --prod --base-href https://github.com/nemilshah54/Angular-Demo.git/'
                bat 'ngh'
            }
        }
        
    }
}
