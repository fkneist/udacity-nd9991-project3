pipeline {
    agent any
    stages {
        stage('Upload to AWS') {
            steps {
                withAWS(region:'us-east-2') {
                    s3Upload(file:'index.html', bucket:'udacity-project3-fkneist', path:'index.html')
                }
            }
        }
    }    
}
