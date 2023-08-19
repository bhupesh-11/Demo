pipeline {
  agent any
  stages {
    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Hello World'
          }
        }

        stage('error') {
          steps {
            sleep 5
          }
        }

      }
    }

    stage('Build') {
      steps {
        bat 'echo %date%'
      }
    }

  }
}