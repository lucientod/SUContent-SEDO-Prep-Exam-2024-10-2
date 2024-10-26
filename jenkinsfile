pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat 'dotnet restore'
            }
        }
        stage('Test') {
            steps {
                bat 'dotnet build'
            }
        }
        stage('Deploy') {
            steps {
                bat 'dotnet test'
            }
        }
    }
}
