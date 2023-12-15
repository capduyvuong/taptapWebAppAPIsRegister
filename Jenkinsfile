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
                sh label: 'API Collection Tests', script: 'newman run /taptapWebAppAPIsRegister/Testing - Register flow.postman_collection.json -e //_Environment.postman_environment.json --suppress-exit-code'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
