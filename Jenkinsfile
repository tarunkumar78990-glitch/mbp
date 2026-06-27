pipeline {
  agent any
  stages {
    stage('Use secret') {
      steps {
        withCredentials([string(credentialsId: 'demo-token', variable: 'TOKEN')]) {
          sh 'echo "token length is ${#TOKEN}"' // use it, don't print it
          sh 'echo "the value is $TOKEN"' // watch the log mask it
        }
      }
    }
  }
}
