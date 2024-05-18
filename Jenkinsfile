pipeline {
    agent any

    stages {
        stage('First Repo') {
            steps {
                git branch: 'main', url: 'https://github.com/RawdaMohammad/task2.git'
            }
        }
        stage('Repo 1') {
            steps {
                // Execute the first batch script
                bat 'list_files.bat'
            }
        }
        stage('Second Repo') {
            steps {
                git url: 'https://github.com/kholoudKamkhli/Jenkins'
            }
        }
        stage('Repo 2') {
            steps {
                // Execute the second batch script
                bat 'batch_file.bat'  // Assuming this script is a batch file to be executed on a Windows agent
            }
        }
    }
}