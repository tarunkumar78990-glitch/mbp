pipeline {
  agent any
  stages {
    stage('Tests') {
      parallel {
        stage('Unit') {
          steps {
            sh 'echo unit;  sleep 5'
          }
        }
        stage('Lint') {
          steps {
            sh 'echo lint;  sleep 5'
          }
        }
        stage('Intg') {
          steps {
            sh 'echo intg;  sleep 5'
          }
        }
      }
    }
  }
}
