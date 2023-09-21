pipeline {
    agent any

    stages {
        stage('docker build') {
            steps {
                script {
                    sh "docker build --file homero_pipeline/Dockerfile --target enriquegzmn/homer_page:1.0.0-${BUILD_ID} homero_pipeline"
                }
            }
        }
        stage('docker push') {
            steps {
                script {
                    sh "docker push enriquegzmn/homer_page:1.0.0-${BUILD_ID}"
                }
            }
        }
    }
}