pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                checkout scm
            }
        }

        stage('Execute Bash Script') {
            steps {
                bat './runLs.bat'
            }
        }

    }
}
