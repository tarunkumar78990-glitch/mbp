pipeline {
  agent any
  stages {
    stage('CI') {
      steps {
        echo "Building branch ${env.BRANCH_NAME}"
        sh 'echo build && echo test'
      }
    }
  }
}
