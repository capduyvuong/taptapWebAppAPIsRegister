pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                sh label: 'API Collection Tests', script: 'newman run /taptapWebAppAPIsRegister/Testing-Registerflow.postman_collection.json -e /taptapWebAppAPIsRegister/[STAG]taptap-webapp-proxy.postman_environment.json --suppress-exit-code'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
