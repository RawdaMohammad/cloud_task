pipeline {
    agent any

    stages {
        stage('Checkout 1') {
            steps {
                git branch: 'main', url: 'https://github.com/RawdaMohammad/task2.git'
            }
        }
        stage('Execute Script 1') {
            steps {
                // Execute the first batch script
                bat 'list_files.bat'
            }
        }
        stage('Checkout 2') {
            steps {
                git url: 'https://github.com/kholoudKamkhli/Jenkins'
            }
        }
        stage('Execute Script 2') {
            steps {
                // Execute the second batch script
                bat 'batch_file.bat'  // Assuming this script is a batch file to be executed on a Windows agent
            }
        }
    }
}