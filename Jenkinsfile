pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/Nada-Yasser6612/20216110.git'
            }
        }
        stage('Execute Script') {
            steps {
                bat 'C:\\Program Files\\Git\\bin\\bash.exe runLs.sh'
            }
        }
    }
}
