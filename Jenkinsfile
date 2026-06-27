pipeline {
  agent any
  parameters {
    choice(name: 'ENVIRONMENT', choices: ['dev','prod'])
  }
  stages {
    stage('Always') {
      steps {
        echo 'runs every time'
      }
    }
    stage('Prod only') {
      when {
        expression {
          params.ENVIRONMENT == 'prod'
        }
      }
      steps {
        echo 'only when prod selected'
      }
    }
  }
}
