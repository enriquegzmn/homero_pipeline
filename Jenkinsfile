pipeline {
    agent any

    stages {
        stage('docker build') {
            steps {
                script {
                    sh "docker start -d --name homerpage_container -p 80:80 homerpage:1"
                }
            }
        }
        
    }
}