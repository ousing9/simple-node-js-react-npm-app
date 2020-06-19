pipeline {
    agent {
        docker {
            image 'node:12' 
            args '-p 3000:3000' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'npm config set registry https://registry.npm.taobao.org'
                sh 'npm install' 
            }
        }
    }
}
