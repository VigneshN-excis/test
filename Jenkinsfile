pipeline {
    agent any
    stages {
        stage('PULL') { steps { git 'https://github.com/VigneshN-excis/test.git'} }
        stage('npm') { steps { node('Nodejs14.17'){ bat "npm install" } } }
        stage('build') { steps { bat "ng build" } }
    }
}
