pipeline {
  agent any
  stages {
    stage('Deploy') {
      steps {
        timeout(time: 5, unit: 'MINUTES') {
          input message: 'Deploy to production?', ok: 'Deploy'
        }
        echo 'deploying...'
      }
    }
  }
}
