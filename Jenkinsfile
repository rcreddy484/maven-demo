pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                // Use Maven to build the project
                bat 'mvn clean install'
            }
        }

	stage('Checkstyle Analysis') {
            steps {
                // Run Checkstyle analysis
                // The path to the Checkstyle configuration file may need adjustment based on your project structure
                bat 'mvn checkstyle:checkstyle -Dcheckstyle.config.location=checkstyle.xml'
            }
        }
    }
}
