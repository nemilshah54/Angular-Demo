pipeline {
    agent any

    stages {
        
         
           stage('Compile') {
            steps {
                bat 'node_modules/.bin/ng build' 
            }
        }
      
       stage('Test') {
            steps {
                bat 'node_modules/.bin/ng test --watch=false'
            }
        }
        
    }
}
