pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
                git branch: 'main', url: 'https://github.com/adityamsrit/devops-autofix-app.git'
            }
        }

        stage('Install Backend') {
            steps {
                dir('backend') {
                    bat 'npm install'
                }
            }
        }

        stage('Test Server') {
            steps {
                echo 'Backend setup complete.'
            }
        }
    }
}
