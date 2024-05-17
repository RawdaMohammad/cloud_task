pipeline {
    agent any

    stages {
        stage('All files in directory') {
            steps {
                script {
                    def output = bat(script: 'task.bat', returnStdout: true).trim()
                    echo "Output:\n======\n${output}"
                }
            }
        }
    }
}
