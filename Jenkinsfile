pipeline {
  agent any
  stages {
    stage('01') {
      parallel {
        stage('01') {
          steps {
            sleep 10
          }
        }
        stage('') {
          steps {
            timestamps() {
              sh 'echo(\'a\')'
            }

          }
        }
      }
    }
    stage('02') {
      steps {
        fingerprint 'aaa'
      }
    }
  }
}