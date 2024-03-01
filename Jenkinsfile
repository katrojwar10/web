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
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
    post {
        success {
            mail to: akshaykatrojwar@gmail.com, subject: 'The Pipeline success :('
            
        }
        failure {
            mail to: katrojwarakshay10@gmail.com, subject: 'The Pipeline failed :('
        }
    }
}
