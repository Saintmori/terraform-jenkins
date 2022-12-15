pipeline {
    agent any

    stages {
        stage('apply terraform config') {
            steps {
                sh '''
                terraform init
                terraform plan
                terraform apply -auto-approve
                sh '''
            }
        }
    }
}
