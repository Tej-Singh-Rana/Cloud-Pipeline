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
            sh '''#!/bin/bash

echo -n "Fourth position"'''
          }
        }

      }
    }

  }
}