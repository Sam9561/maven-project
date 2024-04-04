pipeline {
  agent any
  stages {
    stage('Test') {
      steps {
        echo 'hi '
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
        echo 'he deploy-prodc'
      }
    }

    stage('Post-actions') {
      parallel {
        stage('Post-actions') {
          steps {
            echo 'always run'
          }
        }

        stage('success-post') {
          steps {
            echo 'successfull'
          }
        }

        stage('failure') {
          steps {
            echo 'failed one'
          }
        }

      }
    }

  }
}