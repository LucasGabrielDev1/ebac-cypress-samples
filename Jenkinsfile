pipeline {
    agent any

    stages {
        stage('Setup') {
            steps {
               git branch: 'main', url: 'https://github.com/LucasGabrielDev1/ebac-cypress-samples.git'
               bat 'npm install'
            }
        }
               stage('test') {
            steps {
              bat '''set NO_COLOR=1
npm test'''
            }
        }
    }
}
