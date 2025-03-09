pipeline {
    agent any
    environment { 
        DEPLOY_TO = 'production'
        NUMBER = 90
    }
    stages {
        stage('Welcome Step') {
            when { 
                allOf { 
                    environment name: 'DEPLOY_TO', value: 'production'
                    expression { NUMBER > 50 }
                } 
            }
            steps { 
                echo 'Welcome to LambdaTest'
            }
        }
    }
}
