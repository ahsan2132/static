pipeline {
    agent any

    stages {
        stage('Upload to AWS') {
            steps {
              withAWS(region:'eu-east-1') {
                s3Upload(file:'index.html', bucket:'test-static-website-jen', path:'index.html')
              }
            }
        }
    }
}
