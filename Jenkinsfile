pipeline {
    agent any

    stages {
      
      
      stage('Install') {
            steps {
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
                bat 'node_modules/.bin/ng test --progress false --watch false'
            }
        }
        
    }
}
