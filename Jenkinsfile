pipeline {
    agent any

    stages {
        stage('All files in directory') {
            steps {
                script {
		    echo 'Hello World'
		    bat 'task.bat'
                    def output = bat(script: 'task.bat', returnStdout: true).trim()
                    echo "All files:\n${output}"
                }
            }
        }
    }
}
