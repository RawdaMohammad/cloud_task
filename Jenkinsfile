pipeline {
  agent any
  stages {
    stage('Cloud Task') {
      steps {
	def output = bat(script: 'task.bat', returnStdout: true).trim()
        echo "Files:\n======\n${output}"
      }
    }
  }
}
