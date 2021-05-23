pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Welcome to Jenkins Pipeline'
            }
        }
        stage('Install node module') {
          steps {
            node('Nodejs14.17'){
              bat "npm install"              
            }
           }
        }
        stage('Build') {
            steps {
                bat "ng build"               
            }
        }
        stage('Test') {
            steps {
                bat "ng test"
            }
        }
    }
} 
