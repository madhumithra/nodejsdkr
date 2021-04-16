pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                bat 'node -v'
                bat 'npm install'
            }
        }
        
        stage('Test'){
            steps{
                 env.NODE_ENV = "test"
                 print "Environment will be : ${env.NODE_ENV}"
                 bat 'npm test'

             }
        }
        
        
                
    }
}
