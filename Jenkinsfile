pipeline {
  agent any
  stages {
    stage('first') {
      parallel {
        stage('first') {
          steps {
            echo 'Hello'
          }
        }

        stage('second') {
          steps {
            echo 'Second '
          }
        }

      }
    }

  }
}