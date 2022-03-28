pipeline {
  agent any
  stages {
    stage('Test') {
      steps {
        sh '''pwd
date
'''
      }
    }

    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'this is my build stage'
          }
        }

        stage('buildp') {
          steps {
            sh 'pwd'
          }
        }

      }
    }

    stage('deploytotest') {
      steps {
        sh 'cal 2021'
      }
    }

  }
}