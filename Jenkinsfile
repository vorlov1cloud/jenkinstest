pipeline {
  agent any
  stages {
    stage('ok') {
      parallel {
        stage('ok') {
          steps {
            sh 'echo ok1'
          }
        }
        stage('ok2') {
          steps {
            sh 'echo OK2'
          }
        }
        stage('ok5') {
          steps {
            sh 'echo ok5'
          }
        }
      }
    }
    stage('ok3') {
      parallel {
        stage('ok3') {
          steps {
            sh 'echo ok3'
            sh 'echo okok3'
          }
        }
        stage('ok4') {
          steps {
            sh 'echo ok4'
          }
        }
      }
    }
    stage('ok6') {
      steps {
        sh 'echo ok6'
      }
    }
  }
}