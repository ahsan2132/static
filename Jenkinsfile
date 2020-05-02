pipeline {
    agent any

    stages {
        stage('Upload to AWS') {
            steps {
              withAWS() {
                s3Upload(file:'index.html', bucket:'test-static-website-jen', path:'index.html')
              }
            }
        }
    }
}
