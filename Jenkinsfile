pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            bat 'dir'
          }
        }

        stage('build date') {
          steps {
            bat 'echo %date%'
          }
        }

      }
    }

    stage('Test') {
      steps {
        echo 'Testing'
      }
    }

  }
}