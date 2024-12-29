pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                // Cloning the repository (this happens automatically if you're using a Multibranch Pipeline)
                checkout scm
            }
        }

        stage('Set Permissions') {
            steps {
                // Make the script executable (not required on Windows, but keep the stage for cross-platform)
                bat 'echo Setting permissions is not applicable on Windows.'
            }
        }

        stage('Execute Script') {
            steps {
                // Execute the script
                bat 'runLs.bat'
            }
        }
    }
}
