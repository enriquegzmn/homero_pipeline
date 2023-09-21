pipeline {
    agent any

    stages {
        stage('docker build') {
            steps {
                script {
                    sh "docker build -t homerapp:1.0.${BUILD_ID} ."
                }
            }
        }
        stage('docker push') {
            steps {
                script {
                    sh "docker push enriquegzmn/homer_page:1.0.${BUILD_ID}"
                }
            }
        }
    }
}