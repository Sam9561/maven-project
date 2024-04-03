pipeline {
  agent any
  stages {
    stage('Test') {
      steps {
        echo 'hi '
        sh '"maven test"'
      }
    }

    stage('Build') {
      steps {
        echo 'hi build'
      }
    }

    stage('Deploy-on-test') {
      steps {
        echo 'hi deploy-test'
      }
    }

    stage('deploy-on-prod') {
      steps {
        echo 'he deploy-prod'
      }
    }

  }
}