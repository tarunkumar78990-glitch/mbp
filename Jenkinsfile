pipeline {
  agent any
  stages {
    stage('Use secret') {
      steps {
        withCredentials([usernamePassword(credentialsId: 'reg-creds', usernameVariable: 'U', passwordVariable: 'P')]) {
        sh 'echo "user=$U pass is masked: $P"'
      }
        }
      }
    }
  }
}
