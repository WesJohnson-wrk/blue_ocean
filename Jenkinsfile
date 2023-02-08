pipeline {
  agent any
  stages {
    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo '"testing"'
          }
        }

        stage('Parallel') {
          steps {
            echo '"Running environment"'
          }
        }

      }
    }

    stage('Build') {
      steps {
        echo '"Building Environment"'
      }
    }

    stage('Final') {
      steps {
        echo '"Clean up"'
      }
    }

  }
}