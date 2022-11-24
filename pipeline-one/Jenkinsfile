pipeline {
    agent any

    stages {
        stage('Configure') {
            steps {
                echo 'Configuring...'
            }
        }
        stage('Clone') {
            steps {
                echo 'Cloning...'
            }
        }
        stage('Build') {
            steps {
                echo 'Building...'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                catchError(buildResult: 'SUCCESS', stageResult: 'FAILURE') {
                    sh "exit 1"
                }
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
            }
        }
        stage('Publish') {
            steps {
                echo 'Publishing...'
            }
        }
    }
}
