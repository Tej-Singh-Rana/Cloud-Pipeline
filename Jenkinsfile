pipeline {
  agent any
  stages {
    stage('first') {
      parallel {
        stage('first') {
          steps {
            echo 'Second Testing'
          }
        }

        stage('second') {
          steps {
            echo 'After failed previous testing repeated again'
            sleep 2
            echo 'On process'
          }
        }

        stage('third') {
          steps {
            sleep(time: 2, unit: 'NANOSECONDS')
          }
        }

        stage('fourth') {
          steps {
            echo 'Cool Down'
          }
        }

      }
    }

    stage('five') {
      parallel {
        stage('fifth') {
          steps {
            echo 'count down'
          }
        }

        stage('sixth') {
          steps {
            sleep 5
          }
        }

      }
    }

  }
  environment {
    CLUSTER_NAME = 'KUBERNETES'
  }
}