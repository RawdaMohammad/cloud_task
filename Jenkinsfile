pipeline {
    agent any

    stages {
        stage('All files in directory') {
            steps {
                script {
                    echo 'Hello World'
                    def output = bat(script: 'task.bat', returnStdout: true).trim()
                    
                    // Filter out the directory path
                    def lines = output.readLines().findAll { it !=~ /^.*>task\.bat$/ }
                    // Print only filenames
                    echo "All files:\n${lines.join('\n')}"
                }
            }
        }
    }
}
