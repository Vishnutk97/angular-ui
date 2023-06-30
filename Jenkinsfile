pipeline {
    agent {
      label 'jenkins-slave' 
    }
    stages {
        stage('Install') {
            steps {
                sh "npm install"
            }
        }
        
        stage('Build') {
            steps {
                sh "npm run build"
            }
        }

        stage('Deploy') {
            steps {
                sh "npm run deploy"
            }
        }
    }
}
