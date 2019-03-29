pipeline {
  agent any
  stages {
    stage('Buzz Build') {
      steps {
        sh '''sleep 2
echo done.

'''
      }
    }
    stage('Testing A') {
      parallel {
        stage('Buzz Test') {
          steps {
            sh '''sleep 3
echo done.'''
          }
        }
        stage('Testing B') {
          steps {
            sh '''sleep 6
echo done.'''
          }
        }
      }
    }
  }
}