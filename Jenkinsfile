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

        stage('third') {
          steps {
            sleep(time: 2, unit: 'NANOSECONDS')
          }
        }

        stage('fourth') {
          steps {
            timestamps()
          }
        }

      }
    }

    stage('five') {
      steps {
        echo 'count down'
      }
    }

  }
}