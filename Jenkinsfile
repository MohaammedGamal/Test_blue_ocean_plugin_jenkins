pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build completed ...'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Test completed ...'
          }
        }

        stage('Notify') {
          steps {
            echo 'Notification sent ...'
          }
        }

      }
    }

  }
}