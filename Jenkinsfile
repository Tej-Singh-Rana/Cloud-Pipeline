pipeline {
  agent any
  stages {
    stage('first') {
      parallel {
        stage('first') {
          steps {
            sh 'echo "Second testing"'
          }
        }

        stage('second') {
          steps {
            sh '''sleep 5
echo "Hello Edited Message"
echo ""
echo "Again trial"'''
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
}