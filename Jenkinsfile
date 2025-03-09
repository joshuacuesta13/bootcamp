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
                    equals(actual: currentBuild.number, expected: 1)                } 
            }
            steps { 
                echo 'Welcome to LambdaTest'
            }
        }
    }
}
