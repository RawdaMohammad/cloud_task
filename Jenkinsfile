pipeline {
    agent any

    stages {
        stage('All files in directory') {
            steps {
                script {
		    echo 'Hello World'
                    def output = bat(script: 'task.bat', returnStdout: true).trim()
                    echo "All files:\n${output}"
                }
            }
        }
    }
}
