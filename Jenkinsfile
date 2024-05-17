pipeline {
  agent any
  stages {
    stage('Cloud Task') {
      script {
	echo 'Hello World"
        def output = bat(script: 'task.bat', returnStdout: true).trim()
        echo "List of Files:\n${output}"
      }
    }
  }
}
