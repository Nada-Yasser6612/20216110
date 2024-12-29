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
                // Make the script executable
                sh 'chmod +x runLs.sh'
            }
        }

        stage('Execute Script') {
            steps {
                // Execute the script
                sh './runLs.sh'
            }
        }
    }
}
