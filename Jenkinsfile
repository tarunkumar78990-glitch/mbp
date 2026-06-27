pipeline {
  agent any
  stages {
    stage('Use secret') {
      steps {
        withCredentials([usernamePassword(credentialsId: 'passwd-slave-jenkins-', usernameVariable: 'U', passwordVariable: 'P')]) {
        sh 'echo "user=$U pass is masked: $P"'
      }
        }
      }
    }
  }
}
