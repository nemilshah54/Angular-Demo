pipeline {
    agent any

    stages {
      
      
      stage('Install') {
            steps {
                bat 'npm i puppeteer' 
                bat 'npm install'
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
      
      stage('Publish') {
            steps {        
               bat 'del sample.content'
               bat '7z a -tzip sample.content -r dist'
            }
        }
        
    }
}
