pipeline {
    agent any

    stages {
        stage('All files in directory') {
            steps {
                script {
		    echo 'Hello World'
                    sh 'chmod +x task.sh'
                    def output = sh(script: 'task.sh', returnStdout: true).trim()
                    echo "Files:\n======\n${output}"
                }
            }
        }
    }
}
