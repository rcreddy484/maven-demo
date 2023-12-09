pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                // Use Maven to build the project
                sh 'mvn clean install'
            }
        }

        stage('Test') {
            steps {
                // Run any tests here if needed
                sh 'mvn test'
            }
        }

        stage('Deploy') {
            steps {
                // You can add deployment steps here if needed
            }
        }
    }
}
