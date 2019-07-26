pipeline {
    agent any

    stages {
      
      
      stage('Install') {
            steps {
                bat 'npm install --save-dev karma-phantomjs-launcher' 
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
        
    }
}
