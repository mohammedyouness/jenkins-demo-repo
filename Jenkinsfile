pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build completed'
      }
    }

    stage('Test Stages') {
      parallel {
        stage('Test') {
          steps {
            echo 'Test initialized'
          }
        }

        stage('Smoke Testing') {
          steps {
            echo 'Starting Smoke Testing '
          }
        }

        stage('Automation') {
          steps {
            echo 'Starting Automation'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy completed'
      }
    }

  }
}